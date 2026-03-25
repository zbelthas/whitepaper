

# Zbelthas™ System Architecture

## How We Built a Vault You Can Carry in Your Pocket

---

## Table of Contents

- [The Challenge: Security Without Trust](#the-challenge-security-without-trust)
- [The Core Insight: Trust Nothing](#the-core-insight-trust-nothing)
- [The Building Analogy](#the-building-analogy)
- [How It Works in Practice](#how-it-works-in-practice)
- [Platform Security](#platform-security)
- [Why This Matters for You](#why-this-matters-for-you)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## The Challenge: Security Without Trust

Imagine you need to protect something valuable—really valuable. Your life savings. Your most private conversations. Your digital identity.

The traditional approach is to find someone trustworthy and hand them the keys. A bank. A tech company. A cloud provider. You hope they'll protect your valuables better than you could yourself.

But here's the problem: every time you trust someone else with your security, you create a single point of failure. If they get hacked, you get hacked. If they go bankrupt, you lose access. If they decide to change their terms, you have no recourse.

**Zbelthas takes a radically different approach: we built a system where you don't have to trust anyone—not even us.**

This document explains how we achieved that.

---

## The Core Insight: Trust Nothing

Most software is built on a foundation of trust. The operating system trusts the applications. Applications trust their components. Components trust each other. This creates a chain of trust that's only as strong as its weakest link.

Zbelthas inverts this model. We assume that every part of the system could be compromised, and we design accordingly.

### The Untrusted Host

At the center of Zbelthas is what we call the "host"—the main application you interact with. In most software, this would be the most trusted component. In Zbelthas, it's the opposite.

**The host is explicitly untrusted.** It has no access to your private keys. It can't read your messages. It can't make security decisions. All it does is pass messages back and forth between you and the secure components that actually do the work.

Think of it like a receptionist at a high-security facility. They can take your name and direct you to the right office, but they can't access the vault, read classified documents, or make decisions about who gets clearance.

Why design it this way? Because the host is the component most exposed to attack. It handles user input, displays information, and interacts with the outside world. By stripping it of any security-relevant capabilities, we ensure that even if an attacker compromises the host, they gain nothing useful.

### Isolated Workers

The actual security work happens in separate, isolated processes we call "workers." Each worker handles a specific function and runs in its own sandbox:

**The Wallet Worker** manages your cryptocurrency keys and signs transactions. It's the most heavily protected component, running in "deaf" mode—it only accepts commands from the Supervisor and ignores everything else. Your private keys are split using MPC 2-of-3, so the complete key never exists in memory. Hardware security modules (TPM 2.0, Secure Enclave, StrongBox) protect keys even if the worker is compromised.

**The Messaging Worker** handles encrypted communications using the MLS protocol. It manages group encryption keys, encrypts and decrypts messages with perfect forward secrecy, and synchronizes conversations across your devices using CRDT. Voice and video calls are encrypted with post-quantum key exchange (ML-KEM-768) and transmitted peer-to-peer—no servers involved.

**The Browser Worker** provides an isolated environment for web browsing and Web3 dApp interaction. It runs in a separate process with zero persistent storage—no cookies, no history, no cache. When you interact with a dApp, the browser can't access your wallet directly. Instead, it sends requests through the Supervisor, which shows you a native confirmation popup that the browser can't fake or manipulate.

**The P2P Worker** handles network communication for chat and file sharing. It establishes encrypted peer-to-peer connections using libp2p, routes packets between peers, and manages connection pools. All packets are encrypted—the worker never sees plaintext content. It enforces rate limiting and blocks misbehaving peers automatically.

Each worker is physically separated—they don't link against each other's code. If the Browser Worker is compromised, the attacker can't access wallet functions because those functions don't exist in the browser binary. This physical separation provides security guarantees that software isolation alone cannot.

### The Supervisor: The Gatekeeper

Between the untrusted host and the isolated workers sits the Supervisor—a security checkpoint that every request must pass through. Think of it as the customs office at a border crossing.

The Supervisor's job is to verify, route, and audit:

**Verification:** Every request is authenticated with hardware attestation. The Supervisor checks that requests come from legitimate components running in verified sandboxes. Requests without valid attestation are rejected immediately.

**Routing:** Workers can't communicate directly with each other. If the Browser Worker needs the Wallet Worker to sign a transaction, the request flows through the Supervisor. The Supervisor verifies the browser's sandbox, shows you a native confirmation popup, and only then forwards the request to the wallet.

**Auditing:** Every request is logged with a timestamp, source, destination, and result. If something goes wrong, the audit trail shows exactly what happened.

When you sign a transaction from a dApp:

1. The dApp sends a request to the Browser Worker
2. The Browser Worker forwards it to the Supervisor
3. The Supervisor verifies the browser's sandbox is intact
4. The Supervisor shows you a **native confirmation popup** (not web content)
5. You review the transaction details and approve
6. The Supervisor forwards the request to the Wallet Worker with hardware attestation
7. The Wallet Worker verifies the attestation and signs the transaction
8. The signature flows back through the Supervisor to the browser to the dApp

This architecture ensures that even if a malicious dApp compromises the browser, it can't bypass the confirmation popup, fake transaction details, or access wallet keys. The Supervisor acts as an enforcer of security policy that no single component can circumvent.

---

## Hardware Security: Your Device as a Vault

Software security is important, but it has limits. No matter how carefully we write code, software runs on hardware—and hardware can provide security guarantees that software alone cannot.

Zbelthas integrates with the hardware security features built into modern devices:

### On Windows and Linux: TPM 2.0

The Trusted Platform Module is a dedicated security chip that can generate and store cryptographic keys. Keys stored in the TPM never leave the chip—even the operating system can't extract them. Zbelthas uses the TPM to:

- Generate keys that are bound to your specific device
- Sign messages in a way that proves they came from your device
- Protect sensitive data so it can only be accessed on your device

### On Apple Devices: Secure Enclave

Apple's Secure Enclave is a separate processor dedicated to security operations. It has its own encrypted memory and runs its own secure operating system. Zbelthas uses the Secure Enclave to:

- Store cryptographic keys in hardware-protected memory
- Perform signing operations without exposing keys to the main processor
- Verify device integrity before allowing sensitive operations

### On Android: StrongBox

StrongBox is Android's hardware security module, providing similar capabilities to Apple's Secure Enclave. Zbelthas uses StrongBox to:

- Generate and store keys in tamper-resistant hardware
- Perform cryptographic operations in a secure environment
- Protect keys even if the main operating system is compromised

### Why Hardware Matters

Hardware security provides guarantees that software cannot. Even if malware infects your operating system, it cannot extract keys from the hardware security module. Even if an attacker gains complete control of your device's software, the hardware provides a last line of defense.

This is why Zbelthas achieves security comparable to dedicated hardware wallets—we leverage the same hardware security features, just integrated into the device you already own.

---

## Platform Sandboxing: Layers of Isolation

Beyond hardware security, Zbelthas uses every isolation mechanism your operating system provides.

### On Windows

Each worker runs in an AppContainer—Microsoft's strongest application sandbox. AppContainers are completely isolated from the rest of the system. They can't access files, network resources, or other applications unless explicitly permitted.

We also run workers at "Low Integrity Level," which means they can't modify anything on your system, even if they wanted to. And we use Job Objects to limit resource usage, preventing any worker from consuming excessive memory or CPU.

### On macOS and iOS

Apple's App Sandbox provides similar isolation. Each worker runs with minimal entitlements—permissions that specify exactly what the worker can and cannot do. Our wallet worker, for example, can't access the network, can't read files outside its sandbox, and can't communicate with other applications.

We also use Hardened Runtime, which prevents code injection and other runtime attacks. And on macOS, our application is notarized by Apple, providing an additional layer of verification.

### On Android

Android workers run as isolated processes with their own user IDs. They're further restricted by Seccomp-BPF, which limits the system calls they can make. And SELinux provides mandatory access control, enforcing security policies at the kernel level.

### On Linux

Linux workers are sandboxed using Seccomp-BPF, the same technology used by Chrome and other security-conscious applications. This limits workers to a minimal set of system calls, preventing them from accessing files, network, or other resources they don't need.

---

## Communication: Verified at Every Step

In a system where nothing trusts anything else, communication becomes critical. How do you ensure that messages between components are authentic and haven't been tampered with?

Zbelthas uses hardware-attested communication. Every message between components includes a cryptographic signature from the hardware security module. This signature proves:

1. **The message came from the claimed sender.** Hardware signatures can't be forged by software.

2. **The message hasn't been modified.** Any change to the message would invalidate the signature.

3. **The message is fresh.** Each message includes a timestamp and a unique number that prevents replay attacks.

4. **The sender's environment is secure.** The signature proves the sender is running in a properly sandboxed environment.

If any of these checks fail, the message is rejected. If a component fails too many checks, it's locked out entirely. There's no "try again later"—security failures result in immediate shutdown.

### No External Servers

It's important to emphasize: all of this verification happens locally on your device. Zbelthas doesn't communicate with Google, Apple, Microsoft, or any external server to verify security. Everything is self-contained.

This is crucial for privacy. Many "secure" applications phone home to verify device integrity, leaking information about when and how you use them. Zbelthas never does this. Your security is verified locally, by your own hardware.

---

## The Fail-Closed Principle

Throughout Zbelthas, we follow a simple rule: when in doubt, shut down.

Most software tries to be resilient. If something goes wrong, it attempts to recover, to continue operating in a degraded mode, to give the user a chance to fix the problem.

This is exactly wrong for security software. If a security check fails, something is wrong. Maybe it's a bug. Maybe it's an attack. Either way, the safest response is to stop immediately.

In Zbelthas:

- If a worker can't verify its sandbox is active, it shuts down.
- If a message fails attestation, it's rejected.
- If integrity checks fail, the application terminates.
- If hardware security isn't available, sensitive operations are blocked.

There's no fallback mode. No "continue anyway" option. No degraded security. Either everything works correctly, or nothing works at all.

This might seem extreme, but it's the only way to provide real security guarantees. A system that continues operating when security checks fail is a system that can be attacked by making security checks fail.

---

## What This Means for You

All of this architecture serves a single purpose: protecting you without requiring you to trust anyone.

**Your keys are protected by hardware.** Even if malware infects your device, it can't extract keys from the hardware security module.

**Your data is isolated.** Each component of Zbelthas runs in its own sandbox, unable to access data from other components.

**Communication is verified.** Every message is cryptographically signed and checked, preventing tampering and replay attacks.

**Failures are safe.** If anything goes wrong, Zbelthas shuts down rather than operating in an insecure state.

**No external dependencies.** All security verification happens locally. No servers, no cloud services, no third parties.

The result is security that doesn't depend on trusting us, trusting your operating system vendor, or trusting anyone else. The architecture itself provides the guarantees.

---

## Learn More

This document explains the high-level architecture of Zbelthas. For more details on specific aspects:

- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — How we protect your data mathematically
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense protecting you
- [**Wallet & Blockchain**](05_WALLET_AND_BLOCKCHAIN.md) — How multi-chain support works
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Why our architecture provides regulatory clarity

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon  and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract. The contract only receives donations—no tokens are issued, no rewards are promised.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*


---
Title: Zbelthas - System Architecture
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.

