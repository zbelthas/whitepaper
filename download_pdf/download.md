

# Zbelthas™ Executive Summary

## The Future of Digital Asset Security — In Two Pages

---

## Table of Contents

- [What is Zbelthas?](#what-is-zbelthas)
- [The Problem We Solve](#the-problem-we-solve)
- [Our Solution](#our-solution)
- [Key Technologies](#key-technologies)
- [What We Are Not](#what-we-are-not)
- [Timeline](#timeline)
- [Whitepaper Suite](#whitepaper-suite)
- [Support the Project](#support-the-project)

---

## What is Zbelthas?

Zbelthas is a **complete digital security platform** with three integrated modules: **Wallet**, **Chat**, and **Browser**. It's software that runs entirely on your device, protecting your digital life with military-grade cryptography.

**Key facts:**
- **Three modules, one platform** — Wallet, Chat, and Browser share the same security foundation
- **You control your data** — We never have access to your keys, messages, or browsing history
- **Zero data collection** — No accounts, no tracking, no servers
- **Post-quantum ready** — Protected against future quantum computers
- **Multi-chain wallet** — Bitcoin, Ethereum, Solana, Cosmos, and more
- **Peer-to-peer chat** — Encrypted messaging with no servers or metadata
- **Privacy browser** — Zero persistent storage, fingerprint randomization, Web3 integration

---

## The Problem We Solve

**Today's threats:**
- Exchanges get hacked, users lose funds
- Custodial wallets can freeze your assets
- Current cryptography will break when quantum computers arrive
- Most wallets collect and monetize your data

**Tomorrow's threats:**
- Quantum computers will break Bitcoin's cryptography
- "Harvest now, decrypt later" attacks are already happening
- Regulatory pressure on custodial services is increasing

---

## Our Solution

**Non-custodial architecture:** Your keys never leave your device. We can't access them, freeze them, or lose them.

**Post-quantum cryptography:** We use ML-DSA-87 (NIST's highest security level) combined with classical cryptography. Both must verify—if either fails, the signature is rejected.

**Key splitting (MPC):** Your private key is mathematically split into three pieces. Any two can sign, but no single piece reveals anything. Your complete key never exists in memory.

**Defense in depth:** Eight independent security layers protect your assets. Even if an attacker defeats one, seven more stand in their way.

---

## Key Technologies

| Technology | What It Does | Why It Matters |
|------------|--------------|----------------|
| **ML-DSA-87** | Post-quantum signatures | Protects wallet against quantum computers |
| **ML-KEM-768** | Post-quantum key exchange | Protects chat against quantum computers |
| **MPC 2-of-3** | Key splitting | No single point of failure for wallet keys |
| **MLS Protocol** | Group encryption | Secure chat with perfect forward secrecy |
| **CRDT** | Message synchronization | Serverless chat sync across devices |
| **Hardware Security** | TPM/Secure Enclave/StrongBox | Hardware-level protection on all platforms |
| **Process Isolation** | 4 sandboxed workers | Browser/Chat/Wallet/P2P can't access each other |
| **Zero Storage** | Browser ephemeral mode | No cookies, history, or tracking data |

---

## What We Are Not

**Zbelthas is software — we do not issue, sell, or manage any cryptocurrency, token, or digital asset.**

- We are **not** a cryptocurrency or token
- We are **not** an exchange or trading platform
- We are **not** a custodian or financial service
- We are **not** an investment product

We build security software. You use it to protect assets you already own.

---

## Timeline

| Period | Milestone |
|--------|-----------|
| **April 2025** | Development begins |
| **Q2-Q3 2025** | Core security architecture |
| **Q4 2025** | Multi-platform development |
| **Q1 2026** | Testing and refinement |
| **March 2026** | Private release |
| **2026+** | Continuous improvement |

---

## Whitepaper Suite

This Executive Summary is part of a comprehensive documentation suite. Each document explores a different aspect of Zbelthas:

| Document | Description | Reading Time |
|----------|-------------|--------------|
| [Overview and Vision](01_OVERVIEW_AND_VISION.md) | Why Zbelthas exists | 15-20 min |
| [System Architecture](02_ARCHITECTURE.md) | How it's built | 15-20 min |
| [Cryptographic Foundations](03_CRYPTOGRAPHY.md) | The mathematics | 20-25 min |
| [Security Features](04_SECURITY_FEATURES.md) | Eight layers of defense | 15-20 min |
| [Platform Features](05_PLATFORM_FEATURES.md) | Wallet, Chat, Browser overview | 15-20 min |
| [Legal & Compliance](06_LEGAL_AND_COMPLIANCE.md) | Privacy and regulation | 15-20 min |
| [Chat & Messaging](07_CHAT_AND_MESSAGING.md) | Secure communication | 15-20 min |
| [Browser & Web3](08_BROWSER_AND_WEB3.md) | Privacy browsing | 15-20 min |
| [Wallet Details](09_WALLET_DETAILS.md) | Multi-chain crypto management | 20-25 min |
| [Glossary](GLOSSARY.md) | Terms explained | Reference |

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

### Traditional Methods

Visit **[zbelthas.com/donate](https://zbelthas.com/donate)** 

### Web3 / Cryptocurrency

For on-chain donations, visit our Web3 portal at **[rpc.zbelthas.com](https://rpc.zbelthas.com)** where you can view and interact with our donation smart contract.

The smart contract is **read-only verifiable** — it only receives donations and has no other functionality. No tokens are issued, no rewards are promised. Your donation is a gift to support open development.

**Note:** Donations do not grant any rights, tokens, equity, or promises of future benefits. They are voluntary contributions to support software development.

---

## Learn More

- **Website:** [zbelthas.com](https://zbelthas.com)
- **Documentation:** [docs.zbelthas.com](https://docs.zbelthas.com)
- **Contact:** Visit the Contacts section on our website

---
Title: Zbelthas - Executive Summary
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.


# Zbelthas™

## The Future of Digital Security is Here

---

## Table of Contents

- [Why We Built Zbelthas](#why-we-built-zbelthas)
- [The Problem We're Solving](#the-problem-were-solving)
- [Our Solution](#our-solution)
- [The Technology Behind Zbelthas](#the-technology-behind-zbelthas)
- [What We Are Not](#what-we-are-not)
- [Development Timeline](#development-timeline)
- [What We Can and Cannot Protect Against](#what-we-can-and-cannot-protect-against)
- [The Zbelthas Promise](#the-zbelthas-promise)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Why We Built Zbelthas

Every day, millions of people trust their digital lives to systems they don't control. Your cryptocurrency sits on an exchange that could be hacked tomorrow. Your private messages pass through servers owned by companies that profit from your data. Your passwords are stored in databases that have been breached dozens of times.

We've all accepted this as normal. It isn't.

The digital world was built on a fundamental compromise: convenience in exchange for control. To use modern services, you hand over your keys—literally and figuratively—to corporations, governments, and third parties who promise to keep them safe. Sometimes they do. Often, they don't.

**Zbelthas exists because we believe you shouldn't have to choose between security and usability, between privacy and convenience, between control and accessibility.**

We built Zbelthas to prove that another way is possible: software that protects you as well as a bank vault, without requiring you to trust a bank.

---

## The Problem We're Solving

### Your Digital Life is Under Siege

The threats to your digital security aren't theoretical—they're happening right now:

**Quantum computers are coming.** Within the next decade, quantum computers will be able to break the encryption that protects nearly everything online today. Every Bitcoin transaction, every encrypted message, every digital signature—all of it will become vulnerable. Most security software hasn't even begun to address this threat.

**Data breaches are epidemic.** In 2024 alone, billions of personal records were exposed. Exchanges holding billions in cryptocurrency have been hacked. Password managers have been compromised. Even government agencies have lost control of sensitive data.

**Custodial services fail.** When you trust a third party to hold your assets, you're betting on their security, their solvency, and their honesty. History shows this bet often loses. Exchanges collapse. Companies go bankrupt. Insiders steal. And when they do, your assets disappear with them.

**Privacy has become a luxury.** Every app, every service, every platform collects data about you. Your location, your contacts, your habits, your finances—all of it feeds into profiles that are bought, sold, and exploited. True privacy has become nearly impossible to achieve.

### The False Choice

Until now, you've had two options:

**Option 1: Convenience with risk.** Use standard software wallets, messaging apps, and browsers. They're easy to use, but they collect your data, depend on servers you don't control, and offer limited security against sophisticated attacks.

**Option 2: Security with friction.** Buy expensive hardware wallets, use air-gapped computers, manage complex key ceremonies. You get better security, but at the cost of usability, portability, and significant expense.

Neither option is acceptable. You shouldn't have to be a security expert to protect your digital life. You shouldn't have to spend hundreds of dollars on specialized hardware. And you certainly shouldn't have to sacrifice your privacy just to participate in the digital economy.

---

## What is Zbelthas?

Zbelthas is a complete digital security platform with three integrated modules: **Wallet**, **Chat**, and **Browser**. Each module provides bank-level protection without requiring you to trust anyone—not even us.

### Module 1: Cryptocurrency Wallet

A non-custodial multi-chain wallet supporting Bitcoin, Ethereum, Solana, Cosmos, Polygon, Avalanche, Arbitrum, and Optimism.

**What you can do:**
- Send and receive cryptocurrency across many blockchains
- Sign transactions with hardware-backed keys (TPM 2.0, Secure Enclave, StrongBox)
- Interact with DeFi protocols and decentralized applications
- Manage tokens, NFTs, and multi-chain assets
- Backup with encrypted recovery phrases

**What makes it secure:**
- Your private keys are split using multi-party computation (MPC 2-of-3)—no single piece reveals anything
- Post-quantum hybrid signatures (ML-DSA-87) protect against future quantum computers
- Your complete key never exists in memory during signing
- Hardware security modules protect keys even if your device is compromised

### Module 2: Peer-to-Peer Encrypted Chat

A serverless messaging system with perfect forward secrecy and zero metadata collection.

**What you can do:**
- Send encrypted text messages, voice messages, and files up to 5GB
- Make peer-to-peer video calls with end-to-end encryption
- Create group chats with up to 1000+ participants
- Set messages to automatically delete after a specified time
- Verify contacts with cryptographic fingerprints

**What makes it private:**
- No servers store your messages—everything is peer-to-peer
- MLS protocol (RFC 9420) provides group encryption with forward secrecy
- Post-quantum key exchange (ML-KEM-768) protects against future threats
- We don't know who you talk to, when, or what you say—we have no metadata to collect

### Module 3: Privacy-First Browser

A hardened web browser with zero persistent storage and Web3 integration.

**What you can do:**
- Browse the web without leaving cookies, history, or cache
- Interact with Web3 dApps securely through native wallet integration
- Randomize your browser fingerprint to prevent tracking
- Encrypt DNS queries to hide browsing from your ISP

**What makes it different:**
- Zero persistent storage—nothing survives when you close the browser
- Fingerprint randomization defeats tracking across sessions
- Encrypted DNS-over-HTTPS prevents ISP surveillance
- Sandboxed execution isolates the browser from wallet and chat
- Native transaction confirmations that websites can't fake

### Unified Security Architecture

All three modules share the same security foundation:
- **Memory safety:** Written in Rust with zero unsafe code
- **Process isolation:** Each module runs in its own sandbox
- **Post-quantum cryptography:** ML-DSA-87 signatures, ML-KEM-768 key exchange
- **Hardware security:** TPM/Secure Enclave/StrongBox integration on all platforms
- **Zero trust:** Every component verifies every other component

### What Makes Zbelthas Different

**We can't access your data.** This isn't a policy choice—it's an architectural reality. Zbelthas has no servers that store your information. Your keys, your messages, your browsing history—all of it exists only on your device. We couldn't access it even if we wanted to, even if a court ordered us to, even if someone held a gun to our heads.

**We're ready for quantum computers.** While most security software still relies on encryption that quantum computers will eventually break, Zbelthas uses post-quantum cryptography based on the latest NIST standards (ML-DSA-87 and ML-KEM-768). Your data is protected not just against today's threats, but against tomorrow's as well.

**Your keys are never in one place.** Traditional wallets store your private key as a single piece of data. If an attacker gets that data, they get everything. Zbelthas uses a technique called multi-party computation to split your key into multiple pieces, stored in different locations with different protections. Even if an attacker compromises one piece, they get nothing useful.

**We wrote every line of code with security in mind.** Zbelthas is built in Rust, a programming language designed to eliminate entire categories of security vulnerabilities. We've forbidden the use of any code that could introduce memory safety bugs—the kind of bugs that have caused countless security breaches in other software.

---

## How We Got Here

### Our Journey

**April 2025: The Beginning**

Zbelthas development began with a clear mission: build a post-quantum privacy platform with zero custodial exposure, zero metadata collection, and verifiable security guarantees based on published standards. Not another incremental improvement on existing approaches, but a fundamental rethinking of how digital security should work.

**May–June 2025: Building the Foundation**

We established our cross-platform foundation, ensuring Zbelthas would work seamlessly across Windows, macOS, Linux, Android, and iOS. We built our privacy browser module with fingerprint randomization, encrypted DNS, and zero persistent storage—no cookies, no history, nothing that survives when you close the app.

**July–August 2025: Secure Communication**

Our end-to-end chat module came online with per-message perfect forward secrecy. We achieved a critical milestone: our entire codebase passed a zero-unsafe-blocks audit, confirming that we'd eliminated the vulnerability classes that plague most software—buffer overflows, use-after-free bugs, data races.

**September–October 2025: The Wallet**

We implemented multi-chain wallet support with our distributed key management system. Bitcoin, Ethereum, Solana—all protected by the same rigorous security architecture. Internal testing began with our core team, focusing on key generation correctness and wallet operations across all supported chains.

**November–December 2025: Locking It Down**

Our process-isolation architecture was finalized and verified. We integrated hardware security modules across all platforms—TPM 2.0 on Windows and Linux, Secure Enclave on Apple devices, StrongBox on Android. Cryptographic keys are now hardware-backed, generated inside secure hardware and never exposed to software memory.

**January 2026: Post-Quantum Integration**

ML-DSA-87 and ML-KEM-1024 were fully integrated across all modules. We verified our implementations against official NIST test vectors. The hybrid classical plus post-quantum layers were confirmed operational—defense in depth against both current and future threats.

**February 2026: Going Official**

Zbelthas™ trademark was formally registered, demonstrating our long-term commitment to the project. We established official community channels with verified domain identifiers to prevent impersonation.

**March 2026: Private Release**

The first private build of Zbelthas is now running on Linux. Intensive internal fuzzing tests are in progress across all three modules—Wallet, Chat, and Browser—with focus on cryptographic edge cases and IPC channel security.

---

## Where We're Going

### 2026 Roadmap

**Q1 2026: Core Development & Testing** *(Current Phase)*

We're deep in intensive internal security testing, cryptographic validation, and architecture hardening. Every component is being stress-tested, fuzzed, and verified against our security requirements.

**Q2 2026: Platform Integration**

Cross-platform deployment finalization across Windows, macOS, Linux, Android, and iOS. Hardware security integration will be completed, and we'll polish the user experience to ensure Zbelthas is as intuitive as it is secure.

**Q3 2026: Closed Beta Program**

Limited beta access for early supporters and security researchers. Real-world testing, performance optimization, and final security hardening before public launch. This is where we prove that Zbelthas works not just in our labs, but in the hands of real users.

**Q4 2026: Public Launch**

General availability across all platforms. The full feature set with post-quantum cryptography, hardware-backed security, and non-custodial architecture will be ready for production use.

### Beyond 2026

Our work doesn't stop at launch. We're committed to continuous innovation: regular security updates, new features, and platform expansion. We'll integrate community feedback and implement cutting-edge cryptographic research as it becomes available.

**A note on our timeline:** These dates represent our target schedule. We will delay release if third-party security audits aren't completed or if we discover issues that need to be addressed. We prioritize security over speed—no release will occur without proper validation.

---

## The Technology Behind Zbelthas

You don't need to understand the technical details to use Zbelthas—it's designed to be as simple as any other app. But for those who want to know what's protecting their data, here's an overview of the key technologies.

### Post-Quantum Cryptography

Most encryption used today relies on mathematical problems that are hard for classical computers to solve. Quantum computers will eventually solve these problems easily, breaking the encryption that protects everything from bank transactions to state secrets.

Zbelthas uses ML-DSA-87 for digital signatures and ML-KEM-768 for key exchange—algorithms specifically designed to resist quantum attacks. These aren't experimental technologies; they're based on standards published by NIST, the U.S. National Institute of Standards and Technology, after years of rigorous evaluation.

We also implement a hybrid approach: every cryptographic operation uses both classical and post-quantum algorithms. Even if one approach is somehow compromised, the other still protects you.

### Distributed Key Protection

In a traditional wallet, your private key exists as a single piece of data. If an attacker gets it, they control your assets. Zbelthas takes a different approach.

Your key is split into multiple pieces using a technique called 2-of-3 threshold signing. Each piece is stored separately, with different protections. To sign a transaction, two pieces must work together—but the complete key is never reconstructed. Even during signing, your full private key never exists in memory.

This means an attacker would need to compromise multiple independent systems to steal your assets. Compromise one piece, and you get nothing useful—mathematically, a single piece reveals zero information about the complete key.

### Hardware Security Integration

On every platform, Zbelthas integrates with hardware security modules:

- **Windows and Linux:** TPM 2.0 (Trusted Platform Module)
- **macOS and iOS:** Secure Enclave
- **Android:** StrongBox

These are dedicated security chips built into your device. Cryptographic keys are generated inside the hardware and never exposed to software. Even if malware compromises your operating system, it can't extract keys from the hardware security module.

### Memory Safety

Most security software is written in languages like C or C++ that make it easy to introduce memory safety bugs—buffer overflows, use-after-free vulnerabilities, and similar issues. These bugs are responsible for the majority of security vulnerabilities in software.

Zbelthas is written entirely in Rust, a language designed to make these bugs impossible. We've gone further: every module in Zbelthas explicitly forbids unsafe code. The compiler itself guarantees that entire categories of vulnerabilities simply cannot exist in our codebase.

---

## Your Privacy, Protected

### Zero Data Collection

Zbelthas doesn't collect data about you. Not some data, not anonymized data, not metadata—zero data.

We don't know who you are. We don't know what you're doing. We don't know who you're talking to, what you're buying, or where you're browsing. We can't know, because that information never leaves your device.

This isn't just a privacy policy—it's an architectural guarantee. There are no servers to store your data, no databases to be breached, no logs to be subpoenaed. The information simply doesn't exist anywhere except on your own device.

### What This Means for You

**No data breaches.** You can't lose data you never collected. When other services are hacked, your Zbelthas data isn't affected because it was never on their servers.

**No surveillance.** Governments, corporations, and criminals can't access data that doesn't exist. There's nothing to subpoena, nothing to hack, nothing to buy.

**No profiling.** Your financial transactions, your messages, your browsing habits—none of it feeds into advertising profiles or risk assessments. Your digital life remains yours.

**True ownership.** Your keys, your data, your control. No one can freeze your assets, censor your messages, or lock you out of your own accounts.

---

## Regulatory Clarity

Because Zbelthas is non-custodial and collects no data, it exists in a fundamentally different regulatory category than most financial and communication services.

**We're not a custodian.** Under EU MiCA regulations, a custodian is someone who safeguards crypto-assets on behalf of clients. Zbelthas doesn't hold your assets—you do. We provide the software; you maintain sole control.

**We're not a data controller.** Under GDPR, a data controller is someone who determines the purposes and means of processing personal data. Zbelthas doesn't process your personal data—everything happens locally on your device.

**We're not a money transmitter.** Under U.S. FinCEN guidance, software that doesn't control user funds isn't a money transmitter. Zbelthas is a tool you use to manage your own assets.

This regulatory clarity benefits you directly. It means Zbelthas can operate without the heavy compliance burdens that force other services to collect your data, verify your identity, and report your activities.

---

## What We Are Not

**Zbelthas is software — we do not issue, sell, or manage any cryptocurrency, token, or digital asset.**

- We are **not** a cryptocurrency or token
- We are **not** an exchange or trading platform
- We are **not** a custodian or financial service
- We are **not** an investment product
- We do **not** issue any coin, token, or NFT

We build security software. You use it to protect assets you already own. There is no "Zbelthas coin" and there never will be.

---

## Security You Can Trust

### Our Security Score: 92/100

We've evaluated Zbelthas against the same criteria used to assess hardware wallets and enterprise security systems. The result: a security score of 92 out of 100—comparable to dedicated hardware wallets, achieved entirely in software.

This score reflects our zero-trust architecture, post-quantum cryptography, memory-safe codebase, hardware security integration, and defense-in-depth approach. It represents the maximum achievable security for a software-only, non-custodial, serverless solution.

### What We Protect Against

**Remote attacks:** Network-based attacks, malware, and remote exploitation attempts are blocked by our sandboxed architecture and encrypted communications.

**Memory attacks:** Techniques like cold boot attacks and memory forensics are defeated by our key protection mechanisms. Your secrets are never stored in a form that can be extracted.

**Reverse engineering:** Our code is protected against analysis and tampering. Attackers can't simply decompile Zbelthas to understand how to attack it.

**Supply chain attacks:** Every release is cryptographically signed. Every dependency is audited. You can verify that the software you're running is exactly what we published.

**Future threats:** Post-quantum cryptography protects you against attacks that don't exist yet but will once quantum computers mature.

### Honest Limitations

Zbelthas is software, and software has inherent limitations. We can't protect against:

**Physical device compromise:** If an attacker has physical access to your unlocked device, no software can fully protect you. Use device encryption, secure boot, and biometric protection.

**User error:** If you share your recovery phrase or fall for a phishing attack, Zbelthas can't save you. Security is a partnership between the software and the user.

**Compromised operating system:** If your OS itself is compromised at a deep level, all software running on it is at risk. Keep your system updated and avoid suspicious software.

We believe in transparency about what we can and cannot protect against. Security theater helps no one.

---

## The Zbelthas Promise

We built Zbelthas because we believe everyone deserves real security—not the watered-down, data-harvesting, trust-us-we're-the-good-guys version that passes for security today.

**You own your keys.** Not us, not an exchange, not a cloud provider. You.

**You control your data.** It never leaves your device, never touches our servers, never becomes someone else's asset to monetize or lose.

**You're protected against tomorrow's threats.** Post-quantum cryptography isn't a marketing buzzword for us—it's a fundamental architectural decision that protects you against attacks that most people haven't even heard of yet.

**You don't need to trust us.** Our architecture is designed so that you don't have to trust anyone. We can't access your data, we can't freeze your assets, we can't comply with demands to hand over information we don't have.

This is what security should look like. This is what privacy should feel like. This is Zbelthas.

---

## Learn More

This document provides an overview of Zbelthas and our vision. For deeper exploration of specific topics, see our companion whitepapers:

- [**System Architecture**](02_ARCHITECTURE.md) — How Zbelthas is built and why it's secure
- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — The mathematics protecting your data
- [**Security Features**](04_SECURITY_FEATURES.md) — Defense in depth explained
- [**Platform Features**](05_PLATFORM_FEATURES.md) — Wallet, Chat, and Browser working together
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Regulatory framework and privacy guarantees
- [**Chat & Messaging**](07_CHAT_AND_MESSAGING.md) — Secure peer-to-peer communication
- [**Browser & Web3**](08_BROWSER_AND_WEB3.md) — Privacy browsing and dApp integration
- [**Glossary**](GLOSSARY.md) — Terms and concepts explained

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon  and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract. The contract only receives donations—no tokens are issued, no rewards are promised.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*


---
Title: Zbelthas - Overview and Vision
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.


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



# Zbelthas™ Cryptographic Foundations

## The Mathematics That Keeps You Safe

---

## Table of Contents

- [Why Cryptography Matters](#why-cryptography-matters)
- [The Quantum Threat: Why We Can't Wait](#the-quantum-threat-why-we-cant-wait)
- [Our Approach: Belt and Suspenders](#our-approach-belt-and-suspenders)
- [Key Splitting: No Single Point of Failure](#key-splitting-no-single-point-of-failure)
- [Memory Protection: Secrets That Can't Be Stolen](#memory-protection-secrets-that-cant-be-stolen)
- [Putting It All Together](#putting-it-all-together)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Why Cryptography Matters

Every time you send a message, sign a transaction, or prove your identity online, you're relying on cryptography. It's the mathematical foundation that makes digital security possible.

But here's what most people don't realize: the cryptography protecting nearly everything online today is living on borrowed time.

Quantum computers—machines that exploit the strange properties of quantum physics—are advancing rapidly. When they become powerful enough, they'll be able to break the encryption that protects your bank account, your messages, your cryptocurrency, and your identity. Not in years. In minutes.

Most security software hasn't even begun to address this threat. Zbelthas has.

This document explains how we protect your data—not just against today's threats, but against tomorrow's as well.

---

## The Quantum Threat: Why We Can't Wait

### How Current Encryption Works

Most encryption today relies on mathematical problems that are extremely hard for computers to solve. For example, if you multiply two very large prime numbers together, it's easy to get the result. But given only the result, figuring out which two primes were multiplied is incredibly difficult—so difficult that even the fastest supercomputers would take longer than the age of the universe to solve it.

This asymmetry—easy in one direction, practically impossible in reverse—is the foundation of modern cryptography.

### Why Quantum Computers Change Everything

Quantum computers don't work like regular computers. They can explore many possibilities simultaneously, using a property called superposition. For certain types of problems—including the mathematical problems that underpin current encryption—this gives them an enormous advantage.

A quantum computer running an algorithm called Shor's algorithm could factor large numbers in hours or days instead of billions of years. This would break RSA, the encryption that protects most internet traffic. It would break elliptic curve cryptography, which protects Bitcoin and Ethereum. It would break the digital signatures that verify software updates, financial transactions, and legal documents.

### The "Harvest Now, Decrypt Later" Attack

Here's the scary part: attackers don't need to wait for quantum computers to be built. They can record encrypted data today and store it. When quantum computers become available, they can decrypt everything they've collected.

This means that sensitive data you're transmitting right now—financial records, medical information, private communications—could be exposed years from now. For data that needs to remain confidential for decades, the quantum threat is already here.

### When Will This Happen?

No one knows exactly when quantum computers will become powerful enough to break current encryption. Estimates range from 5 to 15 years. But cryptographic transitions take time—often a decade or more to fully deploy new standards. If we wait until quantum computers arrive, it will be too late.

That's why Zbelthas implements post-quantum cryptography today.

---

## Post-Quantum Cryptography: Our Defense

### What is Post-Quantum Cryptography?

Post-quantum cryptography uses mathematical problems that are believed to be hard even for quantum computers. Instead of relying on factoring or elliptic curves, these algorithms use problems from lattice mathematics—geometric structures in high-dimensional spaces that remain difficult even with quantum advantages.

### The NIST Standards

The U.S. National Institute of Standards and Technology (NIST) has spent years evaluating post-quantum algorithms. After rigorous analysis by cryptographers worldwide, they've published new standards:

**ML-DSA-87** (also known as Dilithium) for digital signatures. This is what Zbelthas uses to sign transactions and verify authenticity. The "87" indicates Category 5 security—the highest level, equivalent to 256-bit classical security.

**ML-KEM-768** (also known as Kyber) for key exchange. This is what Zbelthas uses to establish secure communication channels for messaging.

These aren't experimental algorithms. They've been analyzed by the global cryptographic community for years and have been standardized by NIST as FIPS 203 and FIPS 204.

### Our Hybrid Approach

Despite our confidence in post-quantum algorithms, we don't rely on them alone. Zbelthas uses a hybrid approach: every cryptographic operation uses both classical and post-quantum algorithms.

When you sign a transaction, Zbelthas creates two signatures: one using classical cryptography (like the algorithms Bitcoin and Ethereum use today) and one using post-quantum cryptography. Both signatures must verify for the transaction to be valid.

Why do this? Defense in depth. If somehow the post-quantum algorithms turn out to have weaknesses we don't know about yet, the classical algorithms still protect you. If quantum computers break the classical algorithms, the post-quantum algorithms still protect you. An attacker would need to break both simultaneously—a much harder task.

---

## Your Keys Are Never in One Place

### The Problem with Traditional Wallets

In a traditional cryptocurrency wallet, your private key exists as a single piece of data. It might be stored in a file, in memory, or on a hardware device. But wherever it is, it's complete—and if an attacker gets it, they control your assets.

This is a fundamental vulnerability. No matter how well you protect that key, it's a single point of failure.

### How Zbelthas Splits Your Key

Zbelthas uses a technique called threshold cryptography to eliminate this vulnerability. Your private key is mathematically split into three pieces, called shares. These shares are stored in different locations with different protections.

Here's the crucial part: **your complete private key never exists.** Not when you create your wallet. Not when you sign a transaction. Not ever.

When you need to sign a transaction, two of the three shares work together mathematically to produce a valid signature—without ever being combined into a complete key. Each share performs part of the computation, and the results are combined to create the final signature.

### What This Means for Security

**If an attacker steals one share, they get nothing.** Mathematically, a single share reveals zero information about your private key. It's not like having one-third of a password—it's like having nothing at all.

**You can lose one share and still access your funds.** Because only two shares are needed to sign, you have redundancy built in. If one share is lost or corrupted, you can still use the other two.

**Compromise requires multiple independent breaches.** An attacker would need to compromise two different storage locations with two different protection mechanisms. This is dramatically harder than compromising one.

---

## Protecting Keys in Memory

### The Memory Dump Problem

Even with distributed keys, there's a moment of vulnerability: when a share is loaded into memory to perform a cryptographic operation. If an attacker can read your device's memory at that moment—through malware, a cold boot attack, or forensic analysis—they might be able to extract the share.

Zbelthas uses multiple techniques to address this:

### Automatic Cleanup

Every piece of sensitive data in Zbelthas is automatically erased from memory the moment it's no longer needed. We don't rely on the operating system's garbage collection, which might leave data in memory indefinitely. We explicitly overwrite sensitive memory with zeros before releasing it.

### Protected Storage

While keys are in use, they're stored in protected memory regions that resist extraction. We use techniques that make it difficult for attackers to locate and read key material even if they can access memory.

### Hardware Protection

On platforms that support it, we store keys in hardware security modules (TPM, Secure Enclave, StrongBox) where they're protected by dedicated security hardware. Keys in these modules can perform cryptographic operations without ever being exposed to the main processor or operating system.

---

## Protecting Against Side Channels

### What Are Side-Channel Attacks?

Sometimes attackers don't need to break the mathematics of cryptography. Instead, they observe how the cryptographic operations are performed—how long they take, how much power they consume, what patterns they create in memory access.

These "side channels" can leak information about secret keys. For example, if a cryptographic operation takes slightly longer when processing a "1" bit versus a "0" bit, an attacker who can measure timing precisely might be able to reconstruct the entire key.

### Constant-Time Operations

Zbelthas implements all cryptographic operations in constant time. This means every operation takes exactly the same amount of time regardless of the data being processed. There are no shortcuts, no early exits, no data-dependent branches.

When comparing two values, we don't stop at the first difference—we always compare every byte. When performing calculations, we don't skip steps even if we could. This eliminates timing side channels.

### Access Pattern Protection

We also protect against attacks that observe which memory locations are accessed. Our key storage uses techniques that make all access patterns look identical, regardless of which key is being used. An attacker watching memory access can't tell which key you're using or what operation you're performing.

---

## Standards and Compliance

### NIST Standards

Zbelthas implements cryptographic algorithms standardized by NIST:

- **FIPS 204 (ML-DSA):** Our post-quantum signature algorithm
- **FIPS 203 (ML-KEM):** Our post-quantum key exchange algorithm  
- **FIPS 197 (AES):** Our symmetric encryption algorithm
- **FIPS 180-4 (SHA-2):** Our hash functions

These standards represent the consensus of the global cryptographic community on secure algorithms and implementations.

### European Regulations

Our cryptographic architecture is designed to meet the requirements of European regulations:

**eIDAS 2.0** establishes requirements for qualified electronic signatures. Our ML-DSA-87 implementation meets Category 5 security requirements, the highest level defined by NIST.

**GDPR** requires appropriate technical measures to protect personal data. Our encryption and key management exceed these requirements.

---

## What This Means for You

You don't need to understand the mathematics to benefit from it. Here's what our cryptographic architecture means in practical terms:

**Your assets are protected against quantum computers.** While most cryptocurrency is vulnerable to future quantum attacks, yours isn't.

**Your keys can't be stolen in one breach.** An attacker would need to compromise multiple independent systems to access your funds.

**Your secrets don't linger in memory.** Sensitive data is automatically erased the moment it's no longer needed.

**Side-channel attacks don't work.** Our constant-time implementations eliminate the subtle leaks that sophisticated attackers exploit.

**You're using proven standards.** Our algorithms have been vetted by the global cryptographic community and standardized by NIST.

This is the mathematical foundation that makes Zbelthas secure—not just today, but for decades to come.

---

## Learn More

This document explains the cryptographic foundations of Zbelthas. For more details on specific aspects:

- [**System Architecture**](02_ARCHITECTURE.md) — How these cryptographic components fit together
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense protecting you
- [**Wallet & Blockchain**](05_WALLET_AND_BLOCKCHAIN.md) — How cryptography enables multi-chain support
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Regulatory implications of our cryptographic choices

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon  and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract. The contract only receives donations—no tokens are issued, no rewards are promised.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*


---
Title: Zbelthas - Cryptographic Foundations
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Security Features

## Eight Layers of Protection Between You and Attackers

---

## Table of Contents

- [Security That Works Like a Medieval Castle](#security-that-works-like-a-medieval-castle)
- [Layer 1: Memory Safety — The Foundation](#layer-1-memory-safety--the-foundation)
- [Layer 2: Operating System Sandbox — The Outer Wall](#layer-2-operating-system-sandbox--the-outer-wall)
- [Layer 3: Key Splitting — The Distributed Vault](#layer-3-key-splitting--the-distributed-vault)
- [Layer 4: Post-Quantum Cryptography — Future-Proof Locks](#layer-4-post-quantum-cryptography--future-proof-locks)
- [Layer 5: Anti-Reverse-Engineering — The Invisible Maze](#layer-5-anti-reverse-engineering--the-invisible-maze)
- [Layer 6: Anti-Tampering — The Alarm System](#layer-6-anti-tampering--the-alarm-system)
- [Layer 7: Supply Chain Security — Trusted Materials](#layer-7-supply-chain-security--trusted-materials)
- [Layer 8: Legal Architecture — The Final Shield](#layer-8-legal-architecture--the-final-shield)
- [Why Eight Layers Matter](#why-eight-layers-matter)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Security That Works Like a Medieval Castle

The best security isn't a single wall—it's many walls, each protecting the next. Medieval castles weren't defended by one barrier; they had moats, outer walls, inner walls, towers, and a keep at the center. An attacker who breached one defense still faced many more.

Zbelthas applies this same principle to digital security. We call it defense in depth: eight independent layers of protection, each designed to stop different types of attacks. Even if an attacker somehow defeats one layer, seven more stand in their way.

This document explains each layer and why it matters for protecting your digital assets.

---

## Layer 1: Memory Safety — The Foundation

### Why Most Software Has Security Holes

The majority of security vulnerabilities in software come from a single source: memory safety bugs. These are programming errors where software accidentally reads or writes to the wrong part of memory. Buffer overflows, use-after-free bugs, null pointer dereferences—these technical-sounding problems are responsible for most of the hacks you read about in the news.

These bugs exist because most software is written in programming languages (like C and C++) that don't prevent them. It's like building a house where the walls might randomly develop holes—you can try to patch them, but new ones keep appearing.

### How Zbelthas Eliminates These Bugs

Zbelthas is written entirely in Rust, a programming language specifically designed to make memory safety bugs impossible. The Rust compiler mathematically proves that certain categories of bugs cannot exist in the code before it ever runs.

We've gone further: every component of Zbelthas explicitly forbids any code that could bypass these safety guarantees. The result is that entire categories of attacks—the ones responsible for most security breaches—simply cannot work against Zbelthas.

This isn't a claim we make lightly. It's a mathematical property of how the software is constructed.

---

## Layer 2: Operating System Sandboxing — Isolation

### Containing the Damage

Even with memory-safe code, we assume that any component could potentially be compromised. That's why each part of Zbelthas runs in its own isolated sandbox, using the strongest isolation mechanisms your operating system provides.

Think of it like a submarine with watertight compartments. If one compartment floods, the others remain dry. If one component of Zbelthas were somehow compromised, it couldn't access the others.

### Platform-Specific Protection

On Windows, we use AppContainer—Microsoft's strongest application sandbox. On macOS and iOS, we use Apple's App Sandbox with minimal permissions. On Android, we use isolated processes with additional restrictions. On Linux, we use Seccomp-BPF, the same technology that protects Chrome.

Each sandbox strictly limits what its component can do. The wallet component, for example, can't access the network. The browser component can't access your keys. Even if malware somehow got inside one component, it would find itself trapped in a box with no way to reach anything valuable.

---

## Layer 3: Distributed Key Protection — No Single Point of Failure

### The Problem with Traditional Key Storage

In most wallets, your private key exists as a single piece of data. Steal that data, and you control everything. It's a single point of failure—one successful attack, and you lose everything.

### How We Eliminate This Vulnerability

Zbelthas splits your key into multiple pieces stored in different locations with different protections. To sign a transaction, multiple pieces must work together—but they're never combined into a complete key.

This means there's no single thing an attacker can steal. They would need to compromise multiple independent systems simultaneously. And even then, the mathematical properties of our key splitting ensure that having some pieces reveals nothing about the others.

---

## Layer 4: Post-Quantum Cryptography — Future-Proof Protection

### The Coming Quantum Threat

Quantum computers will eventually break the encryption that protects most digital assets today. We don't know exactly when, but we know it's coming. Most security software hasn't even begun to address this threat.

### Our Defense

Zbelthas uses post-quantum cryptography based on the latest NIST standards. These algorithms are designed to resist attacks from both classical and quantum computers.

We also use a hybrid approach: every cryptographic operation uses both classical and post-quantum algorithms. Even if one approach is somehow broken, the other still protects you. An attacker would need to break both simultaneously—a much harder task.

---

## Layer 5: Anti-Reverse-Engineering — Protecting the Code Itself

### Why Code Protection Matters

If an attacker can study how security software works, they can find weaknesses to exploit. Reverse engineering—taking apart compiled software to understand its inner workings—is a standard technique for finding vulnerabilities.

### How We Resist Analysis

Zbelthas implements multiple techniques to make reverse engineering extremely difficult. Our security-critical code is transformed in ways that defeat automated analysis tools. The logic that protects your keys is obscured so that even with access to the compiled software, understanding how it works requires enormous effort.

This isn't security through obscurity—our cryptographic algorithms are well-known standards. But the specific implementation details that an attacker would need to exploit are protected against analysis.

---

## Layer 6: Anti-Tampering — Detecting Attacks in Progress

### Active Defense

Security isn't just about building walls—it's also about detecting when someone is trying to breach them. Zbelthas continuously monitors for signs of tampering or attack.

### What We Detect

We detect debuggers—tools that attackers use to analyze running software. We detect modifications to our code. We detect timing anomalies that might indicate someone is trying to extract secrets. We detect attempts to read memory that shouldn't be accessed.

### How We Respond

When tampering is detected, Zbelthas doesn't just log an error and continue. It immediately secures all sensitive data and terminates. There's no "continue anyway" option. If something is wrong, we stop—because continuing in a potentially compromised state is worse than stopping.

---

## Layer 7: Supply Chain Security — Trusting the Software You Run

### The Hidden Threat

Modern software is built from hundreds of components created by different developers. If any of those components is compromised—either by a malicious developer or by an attacker who infiltrates the development process—the entire application becomes vulnerable.

This is called a supply chain attack, and it's increasingly common. You might trust the main developers of an application, but do you trust every developer of every library they use?

### Our Defense

Zbelthas audits every dependency for security issues. We verify that the code we include matches what we expect—no hidden modifications. We sign every release with post-quantum cryptography so you can verify that the software you're running is exactly what we published.

We also support reproducible builds: anyone can compile our source code and verify that they get exactly the same result as our official releases. This proves we haven't hidden anything in the compiled software that isn't in the source code.

---

## Layer 8: Legal and Regulatory Architecture — Protection by Design

### Security Through Architecture

The final layer isn't technical—it's architectural. Because Zbelthas is non-custodial and collects no data, many attack vectors simply don't exist.

There's no server to hack because there is no server. There's no database of user information to steal because we don't collect user information. There's no way for us to freeze your assets or comply with seizure orders because we don't control your assets.

This architecture also provides regulatory clarity. We're not a custodian under financial regulations. We're not a data controller under privacy regulations. This isn't a loophole—it's a fundamental property of how Zbelthas is designed.

---

## Hardware Security: Your Device as a Vault

### Beyond Software Protection

Software security has limits. No matter how carefully we write code, it runs on hardware—and hardware can provide security guarantees that software alone cannot.

Zbelthas integrates with the hardware security features built into modern devices:

**TPM 2.0** on Windows and Linux provides hardware-backed key storage and cryptographic operations. Keys stored in the TPM can never be extracted, even by the operating system.

**Secure Enclave** on Apple devices provides similar capabilities with Apple's dedicated security processor.

**StrongBox** on Android provides hardware-backed security using dedicated security chips.

### What Hardware Security Provides

Hardware security modules can generate and store cryptographic keys in a way that makes extraction physically impossible. They can perform cryptographic operations without ever exposing the keys to software. They can verify the integrity of the software running on the device.

This is why Zbelthas achieves security comparable to dedicated hardware wallets—we leverage the same hardware security features, just integrated into the device you already own.

---

## The Fail-Closed Principle

### When in Doubt, Stop

Throughout all eight layers, Zbelthas follows a simple rule: when something goes wrong, stop immediately.

Most software tries to be resilient—to recover from errors, to continue in a degraded mode, to give users a chance to fix problems. This is exactly wrong for security software.

If a security check fails, something is wrong. Maybe it's a bug. Maybe it's an attack. Either way, the safest response is to stop immediately and protect whatever secrets might be at risk.

In Zbelthas:
- If integrity checks fail, we stop.
- If tampering is detected, we stop.
- If hardware security isn't available, sensitive operations are blocked.
- If attestation fails, we stop.

There's no "continue anyway" option. Either everything works correctly, or nothing works at all. This might seem extreme, but it's the only way to provide real security guarantees.

---

## Our Security Score: 92/100

We've evaluated Zbelthas against the same criteria used to assess hardware wallets and enterprise security systems. The result: a security score of 92 out of 100.

This puts Zbelthas in the same category as dedicated hardware wallets—but achieved entirely in software, running on the device you already own.

### What This Score Means

**92/100** represents the maximum achievable security for a software-only, non-custodial, serverless solution. The remaining 8 points would require dedicated hardware (like an air-gapped HSM) or external security audits that are still pending.

### Honest Limitations

We're transparent about what we can and cannot protect against:

**We protect against:** Remote attacks, malware, memory forensics, reverse engineering, supply chain attacks, timing attacks, and future quantum computers.

**We cannot fully protect against:** Physical access to an unlocked device, user error (like sharing recovery phrases), or a deeply compromised operating system.

Security is a partnership between the software and the user. We provide the strongest protection possible; you need to protect your device and your recovery materials.

---

## What This Means for You

You don't need to understand all eight layers to benefit from them. Here's what they mean in practical terms:

**Your assets are protected by multiple independent defenses.** An attacker would need to defeat all eight layers to compromise your security. Defeating one or two isn't enough.

**Your keys are protected by hardware.** Even if malware infects your device, it can't extract keys from the hardware security module.

**Your software verifies itself.** Zbelthas checks its own integrity and stops if anything is wrong.

**Attacks are detected and stopped.** We don't just build walls—we watch for attackers and respond when we see them.

**The software you run is verified.** You can confirm that Zbelthas hasn't been tampered with.

**Your protection is future-proof.** Post-quantum cryptography protects you against threats that don't exist yet.

This is defense in depth: not one wall, but eight. Not hoping attacks won't happen, but assuming they will and preparing accordingly.

---

## Learn More

This document explains the security features of Zbelthas. For more details on specific aspects:

- [**System Architecture**](02_ARCHITECTURE.md) — How these security layers fit together
- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — The mathematics protecting your data
- [**Wallet & Blockchain**](05_WALLET_AND_BLOCKCHAIN.md) — How multi-chain support works securely
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Regulatory implications of our security architecture

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon  and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract. The contract only receives donations—no tokens are issued, no rewards are promised.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*


---
Title: Zbelthas - Security Features
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Platform Features

## Wallet, Chat, and Browser Working Together

---

## Table of Contents

- [The Complete Platform](#the-complete-platform)
- [Wallet: Multi-Chain Asset Management](#wallet-multi-chain-asset-management)
- [Chat: Secure Peer-to-Peer Messaging](#chat-secure-peer-to-peer-messaging)
- [Browser: Privacy-First Web Access](#browser-privacy-first-web-access)
- [How They Work Together](#how-they-work-together)
- [Getting Started](#getting-started)
- [Security Best Practices](#security-best-practices)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## The Complete Platform

Zbelthas is a unified security platform with three integrated modules: **Wallet**, **Chat**, and **Browser**. Each module is designed to work independently, but they share the same security architecture and can work together seamlessly.

This document provides an overview of all three modules and explains how they integrate. For detailed information about each module, see the dedicated whitepapers:
- [Wallet Details](09_WALLET_DETAILS.md) — Full details on multi-chain crypto management
- [Chat & Messaging](07_CHAT_AND_MESSAGING.md) — Full details on messaging features
- [Browser & Web3](08_BROWSER_AND_WEB3.md) — Full details on browser features

---

## Wallet: Multi-Chain Asset Management

The Zbelthas Wallet is a non-custodial cryptocurrency wallet supporting 8+ blockchains from a single recovery phrase.

### What You Can Do

**Manage Multiple Blockchains** — Bitcoin, Ethereum, Solana, Cosmos, Polygon, Avalanche, Arbitrum, Optimism. One recovery phrase protects all your assets.

**True Ownership** — Your private keys exist only on your device. We can't freeze your assets, comply with seizure orders, or lose your funds in a hack.

**Hardware-Backed Security** — Keys are protected by TPM 2.0 (Windows/Linux), Secure Enclave (Apple), or StrongBox (Android).

**Key Splitting** — Your private key is mathematically split into three pieces. Any two can sign, but no single piece reveals anything. Your complete key never exists in memory.

**Post-Quantum Protection** — Transactions are signed with both classical and post-quantum cryptography. Both must verify.

### Key Features

- Send and receive across 8+ blockchains
- NFT support on Ethereum and Solana
- Human-readable addresses (ENS, Unstoppable Domains)
- Multi-account support for different purposes
- Cross-chain atomic swaps
- 24-word recovery phrase for backup

For complete details on wallet features, security, backup, and advanced capabilities, see [Wallet Details](09_WALLET_DETAILS.md).

---

---

## Chat: Secure Peer-to-Peer Messaging

The Zbelthas Chat module provides encrypted messaging without servers or metadata collection.

### What You Can Do

**Text Messaging** — Send encrypted messages with perfect forward secrecy. Every message uses a new encryption key.

**Voice Messages** — Record and send voice messages up to 5 minutes, encrypted with post-quantum cryptography.

**Video Calls** — Make peer-to-peer encrypted video calls. No servers relay your video—it goes directly from you to the recipient.

**File Sharing** — Send files up to 5GB, automatically encrypted and transmitted peer-to-peer.

**Disappearing Messages** — Set messages to delete automatically after 5 seconds to 7 days.

**Group Chats** — Create encrypted groups with up to 256 participants using the MLS protocol.

### Why It's Private

**No Servers** — Messages go directly between devices. We don't store them, so we can't lose them in a breach or hand them over to authorities.

**No Metadata** — We don't know who you talk to, when, or how often. The architecture makes metadata collection impossible.

**Post-Quantum** — ML-KEM-768 key exchange protects against future quantum computers.

For complete details, see [Chat & Messaging](07_CHAT_AND_MESSAGING.md).

---

## Browser: Privacy-First Web Access

The Zbelthas Browser provides secure web browsing with Web3 dApp integration.

### What You Can Do

**Privacy Browsing** — Browse without cookies, history, or cache. Everything is erased when you close the browser.

**Fingerprint Randomization** — Your browser fingerprint changes every session, preventing tracking.

**Encrypted DNS** — DNS-over-HTTPS prevents your ISP from seeing which websites you visit.

**Web3 dApps** — Interact with decentralized applications through native wallet integration.

**HTTPS-Only** — Unencrypted HTTP connections are blocked automatically.

### Why It's Secure

**Zero Persistent Storage** — Nothing is saved. No cookies, no history, no cache.

**Isolated Execution** — The browser runs in a separate sandbox, isolated from wallet and chat.

**Native Confirmations** — Transaction confirmations appear in native UI that websites can't fake.

For complete details, see [Browser & Web3](08_BROWSER_AND_WEB3.md).

---

## How They Work Together

The three modules share the same security foundation but remain isolated from each other.

### Shared Security Architecture

All three modules benefit from:
- **Memory safety** — Rust with zero unsafe code
- **Process isolation** — Each module runs in its own sandbox
- **Post-quantum cryptography** — ML-DSA-87 and ML-KEM-768
- **Hardware security** — TPM 2.0, Secure Enclave, StrongBox

### Isolation for Security

The modules can't access each other's data:
- The Browser can't read your wallet keys or chat messages
- Chat can't access your wallet keys or browsing history
- The Wallet only communicates through the Supervisor

This isolation means that compromising one module doesn't compromise the others.

### Integration Where It Matters

When modules need to work together, they communicate through the Supervisor:

**Browser + Wallet:** When a dApp needs to sign a transaction, the browser sends a request through the Supervisor. You see a native confirmation popup, approve the transaction, and the wallet signs it—all without the browser ever accessing your keys.

**Chat + P2P:** When you send a message, the Chat module encrypts it and hands it to the P2P module for transmission. The P2P module sees only encrypted packets—it can't read your messages.

This architecture provides both integration and isolation—modules work together when needed, but remain separated for security.

---

## Learn More

This document provides an overview of all three platform modules. For detailed information:

- [**Chat & Messaging**](07_CHAT_AND_MESSAGING.md) — Complete chat features and security
- [**Browser & Web3**](08_BROWSER_AND_WEB3.md) — Complete browser features and Web3 integration
- [**System Architecture**](02_ARCHITECTURE.md) — How the modules fit together
- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — The mathematics protecting your data
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Regulatory implications

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*

---
Title: Zbelthas - Platform Features
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.
---


# Zbelthas™ Legal & Compliance

## Privacy and Regulation in a Non-Custodial World

---

## Table of Contents

- [Why Architecture Matters for Your Rights](#why-architecture-matters-for-your-rights)
- [The Fundamental Difference: Custodial vs. Non-Custodial](#the-fundamental-difference-custodial-vs-non-custodial)
- [Regulatory Clarity](#regulatory-clarity)
- [Privacy by Design](#privacy-by-design)
- [Your Rights and Responsibilities](#your-rights-and-responsibilities)
- [What We Cannot Do](#what-we-cannot-do)
- [Our Commitment](#our-commitment)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Why Architecture Matters for Your Rights

The way software is built determines what's possible—not just technically, but legally. Zbelthas is designed from the ground up to protect your privacy and give you complete control over your assets. This isn't just a feature; it's an architectural decision with profound legal implications.

This document explains how Zbelthas's non-custodial, serverless architecture provides regulatory clarity and protects your rights as a user.

---

## The Fundamental Difference: Custodial vs. Non-Custodial

### How Traditional Services Work

When you use a traditional cryptocurrency exchange or wallet service, you're trusting them with your assets. They hold your private keys. They control your funds. They can freeze your account, comply with seizure orders, or lose everything in a hack.

These services are custodians—they safeguard assets on your behalf. This creates a web of regulatory obligations:

- They must verify your identity (KYC)
- They must monitor your transactions (AML)
- They must report suspicious activity
- They must comply with court orders
- They must protect your data (and notify you if they fail)

All of this regulation exists because they control your assets. The regulations are designed to ensure they don't abuse that control.

### How Zbelthas Works

Zbelthas is fundamentally different. We don't hold your keys. We don't control your assets. We can't freeze your account because we don't have an account to freeze. We can't comply with seizure orders because we don't have access to comply with.

This isn't a loophole or a technicality—it's the core architecture of how Zbelthas works:

**Your keys exist only on your device.** They're never uploaded to our servers because we don't have servers for this purpose.

**Your transactions are signed locally.** The cryptographic operations happen on your device, not on our infrastructure.

**Your data stays with you.** We don't collect personal information, transaction history, or usage analytics.

This architecture means that most financial regulations simply don't apply to Zbelthas—not because we're evading them, but because the conditions that trigger those regulations don't exist.

---

## What This Means Under European Law

### MiCA: The EU's Crypto Regulation

The Markets in Crypto-Assets Regulation (MiCA) is the EU's comprehensive framework for cryptocurrency. It creates extensive requirements for "Crypto-Asset Service Providers" (CASPs)—companies that provide custody, exchange, or other services involving crypto-assets.

**Zbelthas is not a CASP.** Under MiCA, a custodian is someone who "safeguards and administers crypto-assets on behalf of clients." Zbelthas doesn't safeguard your assets—you do. We don't administer your assets—you do. We provide software; you maintain control.

This means the authorization requirements, custody rules, and prudential standards that apply to exchanges and custodial wallets don't apply to Zbelthas.

### GDPR: Data Protection

The General Data Protection Regulation gives you rights over your personal data and imposes obligations on organizations that collect it. But these obligations only apply to "data controllers"—organizations that determine how personal data is processed.

**Zbelthas is not a data controller.** We don't collect your personal data. We don't process it on servers. Everything happens locally on your device. There's no database of user information to protect, no data to breach, no cross-border transfers to manage.

When you use Zbelthas, you're processing your own data on your own device. Under GDPR, this is considered "purely personal or household activity"—outside the regulation's scope.

### eIDAS 2.0: Digital Identity

The updated European regulation on electronic identification establishes requirements for qualified electronic signatures. Zbelthas's cryptographic architecture—using ML-DSA-87 at the highest security level, with keys under your sole control—is designed to meet these requirements.

This means Zbelthas can potentially be used for legally binding digital signatures, not just cryptocurrency transactions.

---

## What This Means Under US Law

### Not a Money Transmitter

In the United States, money transmitters must register with FinCEN and comply with anti-money laundering requirements. But FinCEN has clarified that software providers who don't control user funds are not money transmitters.

**Zbelthas is a software tool, not a money transmission service.** You maintain full control of your funds at all times. We don't accept money from you to transmit to someone else—you send it yourself, using our software.

This exemption applies at the federal level and in most states. New York's BitLicense, California's Money Transmission Act, and similar state regulations generally don't apply to non-custodial wallet software.

### Not a Securities Service

Zbelthas doesn't provide investment advice, manage portfolios, or execute trades on your behalf. We're not an investment adviser or broker-dealer under SEC regulations. We provide a tool; you make your own decisions.

---

## International Recognition

The distinction between custodial and non-custodial services is recognized globally:

**Switzerland:** FINMA doesn't regulate non-custodial wallet software.

**Singapore:** The Payment Services Act excludes non-custodial services.

**Japan:** Self-custody wallets aren't considered crypto-asset exchanges.

**United Kingdom:** The FCA's crypto perimeter doesn't include non-custodial wallets.

The Financial Action Task Force (FATF), which sets global anti-money laundering standards, explicitly excludes non-custodial wallet software from its definition of Virtual Asset Service Providers (VASPs).

---

## Your Privacy, Protected by Design

### Zero Data Collection

Zbelthas doesn't collect data about you. Not some data, not anonymized data, not metadata—zero data.

We don't know who you are. We don't know what transactions you make. We don't know who you communicate with. We can't know, because that information never leaves your device.

This isn't just a privacy policy—it's an architectural guarantee. There are no servers to store your data, no databases to be breached, no logs to be subpoenaed.

### No Tracking, No Analytics

Many applications collect usage data to improve their products. Zbelthas doesn't. We don't track which features you use, how often you open the app, or what errors you encounter.

This means we can't analyze user behavior to improve the product—a real tradeoff. But it also means there's no data trail that could be compromised, sold, or demanded by authorities.

### Local Security Verification

Zbelthas uses hardware security features to verify device integrity, but this happens entirely locally. We don't communicate with Google, Apple, or any external server to verify your device. All security checks happen on your device, using your device's hardware.

This is important because many "secure" applications phone home for attestation, creating a record of when and how you use them. Zbelthas never does this.

---

## Your Responsibilities

Non-custodial architecture gives you freedom, but freedom comes with responsibility.

### You Control Your Keys

This means you're responsible for backing up your recovery phrase and keeping it secure. If you lose it, no one can help you recover your assets—not us, not anyone.

### You Comply with Laws

You're responsible for complying with the laws that apply to you. This includes:

- **Tax obligations:** Cryptocurrency transactions may be taxable events in your jurisdiction
- **Sanctions compliance:** You should not transact with sanctioned parties or addresses
- **Local regulations:** Some jurisdictions have specific rules about cryptocurrency use

Zbelthas doesn't screen transactions or verify compliance—we can't, because we don't see your transactions. This responsibility falls on you.

### You Secure Your Device

Software security has limits. If your device is compromised at a deep level, or if someone has physical access to your unlocked device, no software can fully protect you. Device security is your responsibility.

---

## What We Cannot Do

Because of our architecture, there are things Zbelthas simply cannot do:

**We cannot recover lost keys.** If you lose your recovery phrase and your device, your assets are permanently inaccessible.

**We cannot reverse transactions.** Blockchain transactions are final. We have no ability to undo them.

**We cannot freeze assets.** We don't control your assets, so we can't freeze them—even if ordered to by a court.

**We cannot provide user data.** We don't have user data to provide—even if subpoenaed.

**We cannot comply with seizure orders.** We have no technical capability to seize assets we don't control.

This isn't defiance of authority—it's simply the reality of non-custodial architecture. We've designed a system where these capabilities don't exist.

---

## Our Commitment

### We Will Not Compromise

If future regulations require us to add backdoors, collect user data, or take custody of assets, we will not comply. We would rather exit a jurisdiction than compromise the security and privacy that define Zbelthas.

This isn't a political statement—it's a recognition that the value of Zbelthas depends on its architecture. A Zbelthas that collects data or controls keys isn't Zbelthas at all.

### We Engage Constructively

We participate in regulatory discussions to help policymakers understand the difference between custodial and non-custodial services. We believe good regulation should distinguish between services that control user assets and software tools that empower users to control their own.

### We're Transparent

We publish transparency reports about our operations. We don't hide behind complexity or legal jargon. We want you to understand exactly how Zbelthas works and what it means for your rights.

---

## The Bottom Line

Zbelthas's non-custodial architecture isn't just a technical choice—it's a legal and ethical one. By ensuring that you control your assets and your data, we've created a system where:

- Most financial regulations don't apply (because we're not a financial service)
- Data protection concerns are minimized (because we don't collect data)
- Your privacy is protected by architecture, not just policy
- Your assets are under your control, not ours

This architecture provides regulatory clarity for us and freedom for you. It's the foundation of everything Zbelthas does.

---

## Important Disclaimer

Zbelthas is non-custodial software. You are solely responsible for securing your private keys. Lost keys cannot be recovered. Transactions are irreversible.

You must comply with all applicable laws and regulations in your jurisdiction, including tax reporting and sanctions compliance.

Zbelthas is a software tool and does not provide investment advice, custody services, or financial services of any kind.

This document is for informational purposes only and does not constitute legal advice. Consult qualified legal and tax professionals for advice specific to your situation.

---

## Learn More

This document explains the legal and compliance framework of Zbelthas. For more details on specific aspects:

- [**Overview and Vision**](01_OVERVIEW_AND_VISION.md) — Why we built Zbelthas
- [**System Architecture**](02_ARCHITECTURE.md) — How non-custodial architecture works technically
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense protecting you
- [**Wallet & Blockchain**](05_WALLET_AND_BLOCKCHAIN.md) — How to use Zbelthas for your digital assets

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*

---
Title: Zbelthas - Legal and Compliance
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Chat & Messaging

## Your Conversations, Your Control, Your Privacy

---

## Table of Contents

- [Why Messaging Needs to Change](#why-messaging-needs-to-change)
- [What is Zbelthas Chat](#what-is-zbelthas-chat)
- [How It Works](#how-it-works)
- [Text Messaging](#text-messaging)
- [Voice Messages](#voice-messages)
- [Video Calls](#video-calls)
- [File Sharing](#file-sharing)
- [Disappearing Messages](#disappearing-messages)
- [Group Conversations](#group-conversations)
- [What Makes It Different](#what-makes-it-different)
- [What We Don't Know About You](#what-we-dont-know-about-you)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Why Messaging Needs to Change

Every day, billions of messages flow through servers owned by tech companies. They promise your conversations are private, but what does that really mean?

**The truth about "private" messaging today:**

Most messaging apps encrypt your messages in transit—but the company still sees who you talk to, when you talk, how often, and where you are when you do it. This metadata reveals more about you than the content of your messages ever could.

Many apps store your messages on their servers "for your convenience." If those servers get hacked, your entire conversation history is exposed. If the company gets a legal demand, they hand over everything they have.

Some apps claim to be "end-to-end encrypted"—but they still require phone numbers, collect contact lists, and track your usage patterns. Your messages might be encrypted, but you're not anonymous.

**The fundamental problem:** When your messages pass through someone else's servers, you're trusting them to protect your privacy. History shows this trust is often misplaced.

**Zbelthas Chat takes a different approach:** No servers. No metadata collection. No trust required.

---

## What is Zbelthas Chat

Zbelthas Chat is a peer-to-peer messaging system where your conversations happen directly between you and the people you're talking to—no servers in between.

### Core Capabilities

**Text Messaging** — Send encrypted messages that only the recipient can read. Every message uses a new encryption key, so even if one key is compromised, past and future messages remain secure.

**Voice Messages** — Record and send voice messages up to 5 minutes long, encrypted with the same military-grade cryptography that protects your text messages.

**Video Calls** — Make encrypted video calls directly to other Zbelthas users. No servers relay your video—it goes straight from you to them, encrypted end-to-end.

**File Sharing** — Send files up to 5GB, automatically split into encrypted chunks and transmitted peer-to-peer. Photos, documents, videos—all protected.

**Disappearing Messages** — Set messages to automatically delete after a specified time, from 5 seconds to 7 days. When they're gone, they're really gone—securely erased from all devices.

**Group Conversations** — Create encrypted group chats with up to 256 participants. Every member's messages are protected by the same cryptography that secures one-on-one conversations.

---

## How It Works

### The Peer-to-Peer Difference

Traditional messaging apps work like this:

```
You → Company's Server → Your Friend
```

The company sees everything: who you talk to, when, how often, message sizes, your location, your contacts.

Zbelthas works like this:

```
You ←→ Your Friend
```

Your messages go directly from your device to theirs. No servers. No intermediaries. No one watching.

### The Technology Behind It

**MLS Protocol (Messaging Layer Security)** — A cryptographic protocol standardized by the Internet Engineering Task Force (IETF) specifically for secure group messaging. It ensures that every participant in a conversation can verify that messages haven't been tampered with and that only intended recipients can read them.

**Post-Quantum Encryption** — Your messages are protected by ML-KEM-768, a post-quantum key exchange algorithm standardized by NIST. Even if quantum computers become powerful enough to break today's encryption, your conversations remain secure.

**Perfect Forward Secrecy** — Every message uses a new encryption key. If an attacker somehow compromises one key, they can't decrypt past messages or future messages—only that single message.

**CRDT Synchronization** — Your messages sync across all your devices without a central server. Conflict-free Replicated Data Types ensure that messages appear in the correct order on all devices, even if you're offline when they arrive.

---

## Text Messaging

### How It Works for You

Send a message. It's encrypted on your device, transmitted directly to the recipient's device, and decrypted there. Simple.

### What's Happening Behind the Scenes

When you send a message, Zbelthas:

1. Generates a new encryption key for this message
2. Encrypts the message content with that key
3. Encrypts the key itself with the recipient's public key
4. Transmits both the encrypted message and encrypted key directly to the recipient
5. The recipient's device decrypts the key, then uses it to decrypt the message
6. Both devices securely erase the key from memory

This happens in milliseconds. You just see your message appear in the conversation.

### Message Features

**Reactions** — React to messages with emoji. Reactions are encrypted just like messages.

**Replies** — Reply to specific messages in a conversation. The reply is linked to the original message, making it easy to follow complex discussions.

**Read Receipts** — Optionally let others know when you've read their messages. This is opt-in—you control whether to send read receipts.

**Typing Indicators** — Optionally show when you're typing. Like read receipts, this is opt-in and encrypted.

---

## Voice Messages

### Recording and Sending

Press and hold to record a voice message up to 5 minutes long. Release to send. Your voice is encoded using the OPUS codec—the same technology used by professional audio applications—and encrypted before transmission.

### Privacy Protection

Your voice message is encrypted on your device before it's sent. The recipient receives an encrypted file that only their device can decrypt.

Voice messages are stored temporarily on a decentralized network (IPFS) to allow delivery even if the recipient is offline. The files are encrypted—the network can't listen to them. When the message expires or is deleted, it's removed from the network and securely erased from all devices.

---

## Video Calls

### Direct Connection

When you start a video call, Zbelthas establishes a direct encrypted connection between you and the other person. Your video and audio never pass through our servers or anyone else's.

### How It Works

**Peer-to-Peer Connection** — Your device connects directly to the other person's device using libp2p, a battle-tested peer-to-peer networking library. No STUN servers. No TURN relays. No third parties.

**Encrypted Media** — Your video and audio are encrypted using SRTP (Secure Real-time Transport Protocol) with AES-256-GCM. The encryption keys are derived from a post-quantum key exchange, protecting against future quantum computers.

**Quality** — Video calls use the VP9 codec for video and OPUS for audio—the same technologies used by professional video conferencing systems.

### What We Can't See

Because your calls are peer-to-peer and encrypted, we can't see:
- Who you're calling
- When you call
- How long you talk
- What you say
- What you show on video

We literally don't have the technical capability to intercept your calls, even if we wanted to.

---

## File Sharing

### Send Anything

Share photos, documents, videos—any file up to 5GB. Files are automatically split into 1MB chunks, each encrypted separately, and transmitted peer-to-peer.

### How It Works

When you send a file:

1. Zbelthas splits it into 1MB chunks
2. Each chunk is encrypted with a unique key
3. Chunks are transmitted directly to the recipient
4. The recipient's device decrypts and reassembles the chunks
5. All encryption keys are securely erased from memory

If the transmission is interrupted, Zbelthas automatically resumes from where it left off—no need to start over.

### Privacy

Files are encrypted before they leave your device. Even if someone intercepts the transmission, they get encrypted chunks that are useless without the keys—which only you and the recipient have.

---

## Disappearing Messages

### Time-Limited Conversations

Set messages to automatically delete after a specified time. Choose from:

- **5 seconds** — For extremely sensitive information
- **1 minute** — Quick exchanges
- **1 hour** — Temporary conversations
- **24 hours** — Default for privacy-conscious users
- **7 days** — Maximum retention

### How Deletion Works

When a message expires:

1. The message content is overwritten multiple times with random data
2. The encryption keys are securely erased from memory
3. The message is removed from the conversation history
4. All devices in the conversation delete the message simultaneously

This isn't just hiding the message—it's cryptographically erasing it so that it can't be recovered, even with forensic tools.

### View Once

For maximum privacy, use "View Once" mode. The message is deleted immediately after the recipient reads it—no timer, no delay, just instant deletion.

---

## Group Conversations

### Encrypted Groups

Create group chats with up to 256 participants. Every message is encrypted so that only group members can read it.

### How Group Encryption Works

Group encryption is more complex than one-on-one messaging because every participant needs to be able to decrypt messages, but no one outside the group should be able to.

Zbelthas uses the MLS protocol to manage group encryption keys. When someone sends a message:

1. The message is encrypted with the current group key
2. Every group member's device has a copy of this key
3. When someone joins or leaves, the group key is rotated
4. Old keys are securely erased, so departed members can't read new messages

### Group Management

**Add Members** — Invite people to join the group. They receive a secure welcome message that gives them the current group key.

**Remove Members** — When someone leaves or is removed, the group key is rotated. They can no longer decrypt new messages.

**Admin Controls** — Group creators can designate other admins, control who can add members, and manage group settings.

---

## What Makes It Different

### No Servers

Your messages don't pass through our servers or anyone else's. They go directly from you to the recipient. This means:

- We can't read your messages
- We can't hand over your messages to authorities
- We can't lose your messages in a data breach
- We can't be compelled to spy on you

### No Metadata Collection

Most messaging apps claim they can't read your messages—but they can see who you talk to, when, and how often. This metadata is often more revealing than the content.

Zbelthas doesn't collect metadata because we don't have servers that could collect it. We don't know:

- Who you message
- When you message them
- How often you communicate
- Where you are when you send messages
- Who's in your contact list

### Post-Quantum Protection

Most encrypted messaging apps use encryption that will be broken when quantum computers become powerful enough. Zbelthas uses post-quantum cryptography standardized by NIST, protecting your conversations against future threats.

### Perfect Forward Secrecy

If an encryption key is somehow compromised, it can only decrypt a single message—not your entire conversation history. Every message uses a new key, so past and future messages remain secure.

---

## What We Don't Know About You

Because Zbelthas Chat is peer-to-peer and serverless, we literally don't have the technical capability to collect information about you.

**We don't know:**
- Who you talk to
- When you talk to them
- How often you communicate
- What you say
- Where you are when you send messages
- Your contact list
- Your conversation history
- Your group memberships

**We can't:**
- Read your messages
- Listen to your calls
- Access your files
- See your metadata
- Hand over your data to authorities (we don't have it)
- Lose your data in a breach (we don't store it)

This isn't a policy choice—it's an architectural reality. We built the system so that we don't have access to your data, even if we wanted it.

---

## Learn More

This document explains the chat and messaging features of Zbelthas. For more details on specific aspects:

- [**System Architecture**](02_ARCHITECTURE.md) — How the messaging worker fits into the overall security architecture
- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — The mathematics protecting your messages
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense protecting you
- [**Platform Features**](05_PLATFORM_FEATURES.md) — How Chat integrates with Wallet and Browser
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Why serverless architecture provides regulatory clarity

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*

---
Title: Zbelthas - Chat and Messaging
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Browser & Web3

## Browse Without Leaving a Trail

---

## Table of Contents

- [Why Browsing Privacy Matters](#why-browsing-privacy-matters)
- [What is Zbelthas Browser](#what-is-zbelthas-browser)
- [How It Works](#how-it-works)
- [Privacy Features](#privacy-features)
- [Web3 Integration](#web3-integration)
- [What We Don't Track](#what-we-dont-track)
- [Security Isolation](#security-isolation)
- [What Makes It Different](#what-makes-it-different)
- [Limitations and Honest Trade-offs](#limitations-and-honest-trade-offs)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Why Browsing Privacy Matters

Every website you visit, every link you click, every search you make—all of it builds a profile of who you are, what you care about, and what you might do next.

**The reality of web browsing today:**

Your browser knows everything you do online. Most browsers are built by advertising companies that profit from tracking you. They promise privacy features, but those features have limits designed to protect their business model, not your privacy.

Websites track you across the internet using cookies, fingerprinting, and dozens of other techniques. They know which sites you visit, how long you stay, what you click, and where you go next. This data is bought, sold, and used to manipulate your behavior.

Your internet service provider sees every website you visit. Governments can demand this data. Hackers can intercept it. Even with HTTPS, your ISP knows which sites you're accessing.

**The fundamental problem:** The web was built for convenience, not privacy. Every layer—your browser, your ISP, the websites you visit—is designed to collect data about you.

**Zbelthas Browser takes a different approach:** Zero persistent storage. Encrypted DNS. Fingerprint randomization. Complete isolation from your wallet and messages.

---

## What is Zbelthas Browser

Zbelthas Browser is a privacy-first web browser designed for secure interaction with Web3 applications and privacy-conscious web browsing.

### Core Capabilities

**Privacy Browsing** — Browse the web without leaving a trail. No cookies, no history, no cache. When you close the browser, everything is erased.

**Fingerprint Randomization** — Websites can't track you by your browser fingerprint because your fingerprint changes every session.

**Encrypted DNS** — Your DNS queries are encrypted using DNS-over-HTTPS, preventing your ISP from seeing which websites you visit.

**Web3 dApp Integration** — Interact with decentralized applications securely. Your wallet is isolated from the browser—dApps can't access your keys directly.

**HTTPS-Only** — The browser only loads encrypted connections. Unencrypted HTTP sites are blocked automatically.

**Isolated Execution** — The browser runs in a separate sandboxed process, completely isolated from your wallet and chat. Even if a malicious website exploits the browser, it can't access your sensitive data.

---

## How It Works

### The Isolation Architecture

Traditional browsers run in the same process as the rest of your application. If a website exploits a browser vulnerability, it can potentially access everything on your device.

Zbelthas Browser runs in a completely separate sandboxed process:

```
┌─────────────────────────────────────────┐
│         Zbelthas Application            │
├─────────────────────────────────────────┤
│  Wallet (isolated)                      │
│  Chat (isolated)                        │
│  Settings (isolated)                    │
└─────────────────────────────────────────┘
              ↕ (authenticated IPC)
┌─────────────────────────────────────────┐
│      Browser Worker (sandboxed)         │
│  ┌───────────────────────────────────┐  │
│  │   WebView (further isolated)      │  │
│  │   - No direct module access       │  │
│  │   - Strict content security       │  │
│  └───────────────────────────────────┘  │
└─────────────────────────────────────────┘
```

If a malicious website compromises the browser, it's trapped in the sandbox. It can't access your wallet keys, your chat messages, or any other sensitive data.

### Platform-Specific Technology

Zbelthas Browser uses the best web rendering technology available on each platform:

- **Windows:** WebView2 (Chromium-based, separate process)
- **macOS:** WKWebView (WebKit-based, separate process)
- **Linux:** WebKitGTK (WebKit-based)
- **Android:** Android System WebView (isolated process)
- **iOS:** WKWebView (separate process)

All of these technologies provide process isolation, ensuring that the web content runs separately from the rest of Zbelthas.

---

## Privacy Features

### Zero Persistent Storage

When you close Zbelthas Browser, everything is erased:

- **No cookies** — Websites can't track you across sessions
- **No history** — No record of which sites you visited
- **No cache** — No stored copies of web pages
- **No localStorage** — No persistent data from websites
- **No IndexedDB** — No client-side databases

This isn't just clearing your history—it's running in a mode where nothing is saved in the first place.

### Fingerprint Randomization

Websites can identify you by your "browser fingerprint"—a unique combination of your screen size, installed fonts, timezone, language, and dozens of other characteristics.

Zbelthas randomizes these characteristics every session. To websites, you look like a different person each time you browse. They can't build a profile of you because your fingerprint keeps changing.

### Encrypted DNS (DNS-over-HTTPS)

Normally, when you visit a website, your device asks a DNS server to translate the website name into an IP address. This request is unencrypted, so your ISP can see every website you visit.

Zbelthas encrypts all DNS queries using DNS-over-HTTPS (DoH). Your ISP sees encrypted traffic—they can't tell which websites you're visiting.

### HTTPS-Only Mode

The browser automatically blocks unencrypted HTTP connections. If a website doesn't support HTTPS, you can't access it. This prevents attackers from intercepting your browsing or injecting malicious content.

---

## Web3 Integration

### Secure dApp Interaction

Zbelthas Browser lets you interact with Web3 decentralized applications (dApps) without browser extensions or plugins. The wallet integration is built-in and secure.

### How dApp Wallet Requests Work

When a dApp wants to interact with your wallet:

1. The dApp sends a request through the browser
2. The browser forwards the request to the Zbelthas Supervisor
3. The Supervisor verifies the request and shows you a **native confirmation popup**
4. You review the transaction details in the native UI (not in the browser)
5. If you approve, the Supervisor forwards the request to the Wallet Worker
6. The Wallet Worker signs the transaction with hardware-backed keys
7. The signature is returned to the dApp

**Critical security feature:** The confirmation popup is native UI, not web content. A malicious website can't fake it or manipulate what you see.

### What dApps Can and Cannot Do

**dApps CAN:**
- Request your wallet address
- Request transaction signatures
- Send you to other websites
- Display content

**dApps CANNOT:**
- Access your private keys
- Sign transactions without your approval
- Access your chat messages
- Read your browsing history
- Access other tabs or windows
- Bypass the confirmation popup

### Rate Limiting

To prevent abuse, wallet requests from dApps are rate-limited. A malicious dApp can't spam you with hundreds of transaction requests—the system automatically blocks excessive requests.

---

## What We Don't Track

Because Zbelthas Browser uses zero persistent storage and runs in an isolated sandbox, we don't collect data about your browsing.

**We don't know:**
- Which websites you visit
- How long you spend on each site
- What you search for
- Which dApps you use
- Your browsing patterns
- Your interests or preferences

**We don't store:**
- Your browsing history
- Your cookies
- Your cached pages
- Your form data
- Your download history

This isn't a privacy policy—it's an architectural reality. The browser is designed so that this data doesn't exist to collect.

---

## Security Isolation

### Process Separation

The browser runs in a completely separate operating system process from the rest of Zbelthas. This means:

- A browser exploit can't access wallet keys
- A browser exploit can't read chat messages
- A browser exploit can't access other Zbelthas components

The browser process has minimal permissions. It can render web pages and communicate with the Zbelthas Supervisor through an authenticated channel—nothing more.

### Content Security Policy

The browser enforces a strict Content Security Policy (CSP) that blocks:

- Inline JavaScript execution
- Eval and dynamic code execution
- Unsafe script sources
- Inline styles (with limited exceptions)
- External resource loading from untrusted sources

This prevents many common web attacks, including cross-site scripting (XSS) and code injection.

### Sandbox Enforcement

On startup, the browser verifies that it's running in an operating system sandbox:

- **Windows:** AppContainer with low integrity level
- **macOS:** App Sandbox with minimal entitlements
- **Linux:** Seccomp-BPF restrictions
- **Android:** Isolated process with restricted permissions
- **iOS:** App Sandbox with minimal capabilities

If the sandbox isn't detected, the browser refuses to start. This fail-closed behavior ensures that the browser never runs in an insecure environment.

---

## What Makes It Different

### No Tracking by Design

Most browsers claim they don't track you—but they're built by companies that profit from advertising. Privacy features are added on top of a tracking foundation.

Zbelthas Browser is built from the ground up with zero persistent storage. There's nothing to track because nothing is saved.

### Isolated from Sensitive Data

Most Web3 wallets are browser extensions that run inside your browser. If the browser is compromised, the extension can be compromised too.

Zbelthas Browser is completely isolated from the wallet. The wallet runs in a separate process with separate memory. A browser exploit can't access wallet keys because they're not in the same process.

### Native Transaction Confirmation

Most Web3 wallets show transaction confirmations in the browser. A sophisticated attacker can manipulate what you see.

Zbelthas shows transaction confirmations in native UI that the browser can't access or manipulate. What you see is what you're actually signing.

### Fingerprint Randomization

Most privacy browsers try to make everyone look the same. This creates a unique fingerprint—if you're one of the few people using that browser, you stand out.

Zbelthas randomizes your fingerprint every session. You blend into the crowd because you look different each time.

---

## Limitations and Honest Trade-offs

Privacy and security come with trade-offs. We believe in being transparent about what Zbelthas Browser can and cannot do.

### What Doesn't Work

**Cookies and Sessions** — Because we don't store cookies, you can't stay logged into websites across sessions. Every time you open the browser, you start fresh.

**Browser History** — There's no history to search through. If you want to revisit a site, you need to remember the URL or bookmark it externally.

**Cached Content** — Pages load from scratch every time. There's no cache to speed up repeat visits.

**Form Autofill** — The browser doesn't remember form data. You'll need to re-enter information each time.

**Download History** — Downloaded files aren't tracked. You'll need to remember where you saved them.

### Why These Limitations Exist

These aren't bugs—they're the cost of real privacy. Storing cookies, history, and cache would require persistent storage, which would create a tracking profile.

We chose privacy over convenience. If you need persistent sessions and history, use a traditional browser. If you need privacy, use Zbelthas.

### What We're Working On

**Tor Integration** — Planned for Q3 2026. Route your browsing through the Tor network for additional anonymity.

**Custom DNS Providers** — Choose which DNS-over-HTTPS provider to use, or run your own.

**Bookmark Sync** — Encrypted bookmark synchronization across your devices without a central server.

---

## Learn More

This document explains the browser and Web3 features of Zbelthas. For more details on specific aspects:

- [**System Architecture**](02_ARCHITECTURE.md) — How the browser worker fits into the overall security architecture
- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — The mathematics protecting your connections
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense protecting you
- [**Platform Features**](05_PLATFORM_FEATURES.md) — How Browser integrates with Wallet and Chat
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Why zero-storage architecture provides regulatory clarity

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*

---
Title: Zbelthas - Browser and Web3
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Wallet Details

## Your Crypto, Your Control, Your Security

---

## Table of Contents

- [Multi-Chain Support](#multi-chain-support)
- [True Ownership: What Non-Custodial Means](#true-ownership-what-non-custodial-means)
- [How Your Keys Are Protected](#how-your-keys-are-protected)
- [Getting Started](#getting-started)
- [Sending and Receiving](#sending-and-receiving)
- [Backup and Recovery](#backup-and-recovery)
- [Advanced Features](#advanced-features)
- [Security in Practice](#security-in-practice)
- [Learn More](#learn-more)
- [Support the Project](#support-the-project)

---

## Multi-Chain Support

Zbelthas manages assets across all major blockchain networks from a single recovery phrase.

### Supported Blockchains

**Bitcoin** — The original cryptocurrency. Send and receive Bitcoin using the latest address formats, including Taproot for enhanced privacy and lower fees.

**Ethereum** — The world's largest smart contract platform. Manage ETH, interact with decentralized applications, and hold tokens and NFTs.

**Solana** — High-speed blockchain for fast, low-cost transactions. Full support for SOL and SPL tokens.

**Cosmos** — The internet of blockchains. Transfer assets across the Cosmos ecosystem with IBC support.

**Layer 2 Networks** — Polygon, Avalanche, Arbitrum, Optimism, and other networks are supported, with more being added regularly.

You don't need separate wallets for each blockchain. Zbelthas manages them all with a single recovery phrase and unified security.

---

## True Ownership: What Non-Custodial Means

When you use Zbelthas, you're not trusting us—or anyone—with your assets. This is what "non-custodial" means, and it's fundamentally different from how most financial services work.

### The Custodial Problem

When you keep cryptocurrency on an exchange, you don't actually own it. The exchange holds the private keys, which means they control the assets. They can freeze your account, comply with seizure orders, or lose everything in a hack. "Not your keys, not your coins" isn't just a slogan—it's a description of how blockchain ownership works.

### How Zbelthas is Different

With Zbelthas, your private keys exist only on your device. They're never uploaded to our servers (we don't have servers for this purpose). They're never backed up to the cloud. They're never accessible to anyone but you.

This means:

**We can't freeze your assets.** We don't control them.

**We can't comply with seizure orders.** We don't have access to comply with.

**We can't lose your funds in a hack.** There's nothing to hack on our end.

**We can't recover your wallet if you lose your recovery phrase.** This is the tradeoff of true ownership—you bear the responsibility.

This architecture isn't just a feature—it's a fundamental design principle that shapes everything about how Zbelthas works.

---

## How Your Keys Are Protected

Zbelthas doesn't just store your keys—it protects them with multiple layers of security that work together to keep your assets safe.

### Your Key is Never in One Place

Traditional wallets store your private key as a single piece of data. If someone gets that data, they control your assets. Zbelthas takes a different approach.

Your key is mathematically split into three pieces, stored in different locations with different protections. To sign a transaction, two pieces work together—but the complete key is never reconstructed. Even during signing, your full private key never exists in memory.

This means an attacker would need to compromise multiple independent systems to steal your assets. Getting one piece reveals nothing—mathematically, a single piece contains zero information about the complete key.

### Hardware Security Integration

On every platform, Zbelthas integrates with hardware security features:

- **Windows and Linux:** TPM 2.0 protects key material
- **macOS and iOS:** Secure Enclave provides hardware-backed security
- **Android:** StrongBox ensures keys are protected by dedicated hardware

These hardware modules can perform cryptographic operations without ever exposing keys to software. Even if malware compromises your operating system, it can't extract keys from the hardware.

### Post-Quantum Protection

Your transactions are signed with both classical cryptography (the kind used by Bitcoin and Ethereum today) and post-quantum cryptography (designed to resist future quantum computers). Both signatures must verify for a transaction to be valid.

This means your assets are protected not just against today's threats, but against the quantum computers that will eventually break classical encryption.

---

## Getting Started

Setting up Zbelthas takes about five minutes:

1. **Install the app** on your device
2. **Create a new wallet** — Zbelthas generates a secure recovery phrase
3. **Write down your recovery phrase** — 24 words that can restore your wallet on any device
4. **Verify your phrase** — Zbelthas asks you to confirm several words to ensure you wrote them down correctly
5. **Set your PIN or biometric** — For quick, secure access

That's it. Your wallet is ready to use across all supported blockchains.

---

## Sending and Receiving

### Sending Cryptocurrency

Sending crypto is simple:

1. **Select the blockchain** you want to use
2. **Enter the recipient's address** — or scan a QR code
3. **Enter the amount** to send
4. **Review the transaction** — see exactly what you're sending and any fees
5. **Confirm with your PIN or biometric**

The transaction is signed on your device and broadcast to the network. The whole process takes about 30 seconds.

### Receiving Cryptocurrency

To receive crypto, just share your address. Zbelthas generates addresses for each supported blockchain, and you can display them as QR codes for easy scanning.

### Managing Your Portfolio

Zbelthas shows you all your assets in one place:

- **Total portfolio value** in your preferred currency
- **Asset breakdown** showing what you hold on each blockchain
- **Transaction history** for all your accounts
- **Token management** — add custom tokens or hide small balances

---

## Backup and Recovery

Your recovery phrase is the master key to your wallet. With it, you can restore access to all your assets on any device. Without it, lost access is permanent.

### Your Recovery Phrase

When you create a wallet, Zbelthas generates a 24-word recovery phrase. This phrase, combined with industry-standard derivation methods, can regenerate all your private keys for all supported blockchains.

**Write it down on paper.** Don't store it digitally—not in a notes app, not in cloud storage, not in a password manager. Paper can't be hacked remotely.

**Store it securely.** A safe, a safety deposit box, or another secure location. Consider making multiple copies stored in different places.

**Never share it.** Anyone with your recovery phrase controls your assets. No legitimate service will ever ask for it.

### What If You Lose Your Device?

If your device is lost, stolen, or destroyed, your assets are safe. Install Zbelthas on a new device, enter your recovery phrase, and your wallet is restored with full access to all your assets.

### What If You Lose Your Recovery Phrase?

If you lose your recovery phrase and still have access to your device, you can view it again in Zbelthas settings (after authenticating). If you lose both your device and your recovery phrase, your assets are permanently inaccessible. This is the tradeoff of true non-custodial ownership.

---

## Advanced Features

Beyond basic sending and receiving, Zbelthas offers advanced capabilities for users who want more from their wallet.

### Human-Readable Addresses

Instead of copying long strings of letters and numbers, you can send to blockchain domain names:

- **ENS names** like `alice.eth` on Ethereum
- **Unstoppable Domains** like `alice.crypto`
- **Solana Name Service** addresses

Zbelthas resolves these names to blockchain addresses automatically.

### NFT Support

View and manage your NFT collections across Ethereum and Solana. See artwork, metadata, and collection information. Transfer NFTs to other addresses with the same security as any other transaction.

### Multi-Account Support

Create multiple accounts within a single wallet for different purposes—personal, business, savings—each with its own set of addresses but all protected by the same recovery phrase.

### Cross-Chain Swaps

Exchange assets between different blockchains without using centralized exchanges. Atomic swaps ensure that either both sides of the trade complete, or neither does—no counterparty risk.

---

## Security in Practice

All the security features described in our other documents come together in the wallet to protect your assets.

### Every Transaction is Verified

Before any transaction is signed, Zbelthas performs multiple security checks:

- **Integrity verification** ensures the software hasn't been tampered with
- **Hardware attestation** confirms the secure environment is intact
- **Anti-tampering checks** detect any attempts to interfere with the signing process

If any check fails, the transaction is blocked. There's no "continue anyway" option.

### Your Confirmation is Required

Zbelthas never signs transactions automatically. Every transaction requires your explicit confirmation after reviewing the details. You see exactly what you're signing—the recipient, the amount, the fees—before you approve.

### Sensitive Data is Protected

Your keys are protected by multiple layers:

- **Distributed storage** means no single point of failure
- **Hardware security** protects against software attacks
- **Automatic cleanup** ensures sensitive data doesn't linger in memory
- **Session timeouts** lock your wallet after inactivity

### What We Protect Against

Zbelthas protects your assets against:

- **Remote attacks** — malware, network attacks, phishing
- **Memory forensics** — cold boot attacks, memory dumps
- **Future threats** — quantum computers that will break classical encryption
- **Supply chain attacks** — compromised software updates

### Honest Limitations

We're transparent about what we can't protect against:

- **Physical access to an unlocked device** — if someone has your unlocked phone, software can only do so much
- **Your own mistakes** — if you share your recovery phrase or send to the wrong address, we can't help
- **Deeply compromised operating systems** — if your OS itself is controlled by an attacker, all software is at risk

Security is a partnership. We provide the strongest protection possible; you need to protect your device and your recovery phrase.

---

## Learn More

This document provides detailed information about the Zbelthas Wallet. For broader context:

- [**Platform Features**](05_PLATFORM_FEATURES.md) — How Wallet, Chat, and Browser work together
- [**System Architecture**](02_ARCHITECTURE.md) — How the wallet worker fits into the security architecture
- [**Cryptographic Foundations**](03_CRYPTOGRAPHY.md) — The mathematics protecting your keys
- [**Security Features**](04_SECURITY_FEATURES.md) — The eight layers of defense
- [**Legal & Compliance**](06_LEGAL_AND_COMPLIANCE.md) — Why non-custodial architecture matters

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*

---
Title: Zbelthas - Wallet Details
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ - Auditor Notice

**Access to Detailed Technical Documentation**

---

## Overview

This whitepaper suite provides comprehensive documentation of the Zbelthas security platform for public release. The documents focus on educating the community about the technologies, standards, and philosophy behind Zbelthas.

## For Security Auditors and Researchers

If you are a **security auditor**, **penetration tester**, or **security researcher** interested in conducting a detailed security assessment of Zbelthas, additional technical documentation is available under **Non-Disclosure Agreement (NDA)**.

### Detailed Documentation Includes

The complete technical documentation (Yellow Paper) includes:

- **Implementation Details**: Detailed architecture specifications, module structure, and internal component interactions
- **Cryptographic Implementation**: Specific algorithms, parameter choices, and implementation details
- **Security Mechanisms**: Detailed anti-tampering, anti-debug, and code protection implementations
- **Source Code Access**: Complete codebase review under controlled conditions
- **Build and Deployment**: Detailed build process and deployment procedures
- **Testing Infrastructure**: Test suites, fuzzing harnesses, and security validation tools

### Request Access

To request access to detailed technical documentation, please use the contact form on our website at **zbelthas.com** under the **Contacts** section.

We will guide you through the NDA process and schedule a technical briefing.

### Audit Scope

We welcome security audits covering:

- **Cryptographic Implementation**: Verification of post-quantum algorithms, hybrid signatures, key management
- **Architecture Security**: Zero-trust design, isolation mechanisms, policy enforcement
- **Code Quality**: Memory safety, constant-time operations, side-channel resistance
- **Platform Security**: Sandbox enforcement, hardware attestation, anti-tampering
- **Supply Chain**: Dependency analysis, SBOM verification, build reproducibility

### Responsible Disclosure

Zbelthas follows responsible disclosure practices. To report vulnerabilities or coordinate disclosure, please contact us through the **Contacts** section on **zbelthas.com**.

- **Response time**: Within 48 hours for initial acknowledgment
- **Coordination**: Work together on fixes and disclosure timeline
- **Recognition**: Public acknowledgment in security advisories (with permission)

---

## Public Documentation

The current whitepaper suite provides:

- **Architecture Overview**: High-level system design and component interactions
- **Cryptographic Standards**: NIST-compliant algorithms and security properties
- **Security Features**: Defense-in-depth approach and security layers
- **Wallet Functionality**: Multi-chain support and transaction signing
- **Legal Compliance**: Non-custodial architecture and regulatory advantages

---

## Distribution

This whitepaper suite is distributed via:

- **Official Website**: docs.zbelthas.com
- **Cryptographic Verification**: All documents signed with ML-DSA-87

---

## Contact

For all inquiries—general questions, security audits, vulnerability reports, or legal matters—please visit **zbelthas.com** and use the contact form in the **Contacts** section.

---
Title: Zbelthas - Auditor Notice
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Glossary

## Terms and Concepts Explained Simply

This glossary explains the terminology used throughout the Zbelthas whitepapers. We've written these definitions for curious readers, not cryptography experts.

---

## Core Concepts

### Non-Custodial
When you use Zbelthas, you—and only you—control your private keys. We never have access to them. This is fundamentally different from exchanges or custodial wallets, where someone else holds your keys on your behalf. "Not your keys, not your coins" is the principle behind non-custodial design.

### Post-Quantum Cryptography
Mathematical algorithms designed to remain secure even when quantum computers become powerful enough to break today's encryption. Zbelthas uses these algorithms now, protecting your assets against future threats.

### Defense in Depth
The security principle of using multiple independent layers of protection. Like a medieval castle with moats, walls, and towers, Zbelthas implements eight separate security layers. Even if an attacker defeats one, the others still protect you.

### Zero Data Collection
Zbelthas doesn't collect any information about you—not your identity, not your transactions, not your usage patterns. There's no database to breach because there's no database.

### Fail-Closed
When something goes wrong, Zbelthas stops completely rather than continuing in a potentially compromised state. This might seem inconvenient, but it's the only way to guarantee security.

---

## Cryptography Terms

### Private Key
A secret number that proves you own your cryptocurrency. Anyone who has your private key controls your assets. Zbelthas protects this key with multiple layers of security and never lets it exist in one place.

### Public Key
A number derived from your private key that you can share freely. Others use it to send you cryptocurrency or verify your signatures. Unlike your private key, your public key can be shared without risk.

### Recovery Phrase (Seed Phrase)
The 24 words you write down when creating a wallet. These words can regenerate all your private keys. Protect them like you'd protect the keys to a safe deposit box containing everything you own.

### Digital Signature
Mathematical proof that you authorized a transaction. Like a handwritten signature, but impossible to forge without your private key.

### Hybrid Signature
Zbelthas signs every transaction twice: once with classical cryptography (the kind used today) and once with post-quantum cryptography (designed for the future). Both signatures must be valid. This protects you whether quantum computers arrive tomorrow or never.

### ML-DSA-87
The specific post-quantum signature algorithm Zbelthas uses. It's the highest security level (Category 5) in the new NIST standards—the same standards that will protect government secrets.

### Encryption
Scrambling data so only authorized parties can read it. Zbelthas uses AES-256, the same encryption standard used by governments and militaries worldwide.

---

## Key Protection Terms

### Key Splitting (MPC)
Instead of storing your private key as one piece of data, Zbelthas mathematically splits it into three pieces. Any two pieces can sign a transaction, but no single piece reveals anything about your key. This eliminates the single point of failure that makes traditional wallets vulnerable.

### Threshold Signing
The process of signing a transaction using multiple key pieces without ever combining them. Your complete private key never exists in memory, even during signing.

### Hardware Security Module (HSM)
A dedicated chip designed to protect cryptographic keys. Modern devices have these built in: TPM on Windows/Linux, Secure Enclave on Apple devices, StrongBox on Android. Zbelthas uses these chips to provide hardware-level protection.

### Zeroization
Securely erasing sensitive data from memory by overwriting it with zeros. Zbelthas automatically zeroizes all secrets when they're no longer needed, preventing recovery through memory forensics.

---

## Architecture Terms

### Zero-Trust Architecture
A design philosophy where no component trusts any other component. Every request is verified, every message is authenticated. Even internal components treat each other as potentially compromised.

### Sandbox
An isolated environment that restricts what a program can do. Each component of Zbelthas runs in its own sandbox, limiting the damage if any single component is compromised.

### Hardware Attestation
Cryptographic proof that a message came from a specific device's security hardware. Zbelthas uses this to verify that security components haven't been tampered with—and it all happens locally, without contacting any external servers.

---

## Blockchain Terms

### Blockchain
A distributed ledger that records transactions across many computers. Bitcoin, Ethereum, and Solana are different blockchains with different features.

### Transaction
A transfer of cryptocurrency from one address to another. Once confirmed on the blockchain, transactions are permanent and irreversible.

### Address
A string of letters and numbers that identifies where cryptocurrency can be sent. Like an email address, but for money.

### Token
A cryptocurrency that runs on top of another blockchain. For example, many tokens run on Ethereum using the ERC-20 standard.

### NFT (Non-Fungible Token)
A unique digital asset recorded on a blockchain. Unlike regular cryptocurrency (where one Bitcoin equals any other Bitcoin), each NFT is distinct.

### Smart Contract
A program that runs on a blockchain and automatically executes when certain conditions are met. Ethereum popularized smart contracts.

---

## Security Terms

### Side-Channel Attack
An attack that extracts secrets by observing how a system behaves—timing, power consumption, electromagnetic emissions—rather than breaking the cryptography directly. Zbelthas uses constant-time operations to prevent these attacks.

### Memory Forensics
Extracting data from a computer's memory, either while running or after shutdown (cold boot attack). Zbelthas protects against this through key splitting, zeroization, and memory protection techniques.

### Reverse Engineering
Analyzing compiled software to understand how it works. Attackers use this to find vulnerabilities. Zbelthas uses multiple techniques to make reverse engineering extremely difficult.

### Tampering
Modifying software or hardware to change its behavior. Zbelthas continuously monitors for tampering and stops immediately if detected.

### Supply Chain Attack
Compromising software by attacking its development or distribution process—for example, inserting malicious code into a library that the software depends on. Zbelthas audits all dependencies and signs all releases.

---

## Regulatory Terms

### MiCA (Markets in Crypto-Assets)
The EU's comprehensive regulation for cryptocurrency. It creates extensive requirements for "Crypto-Asset Service Providers" (CASPs). Zbelthas is not a CASP because we don't hold your keys or control your assets.

### GDPR (General Data Protection Regulation)
The EU's data protection law. It imposes obligations on organizations that collect personal data. Zbelthas doesn't collect personal data, so these obligations don't apply.

### Non-Custodial Exemption
Because Zbelthas doesn't hold your keys or control your assets, many financial regulations don't apply. We're a software tool, not a financial service.

### KYC (Know Your Customer)
Requirements for financial services to verify customer identity. Because Zbelthas is non-custodial, we don't have KYC requirements—we don't even know who our users are.

---

## Platform Terms

### TPM (Trusted Platform Module)
A security chip in Windows and Linux computers that can store keys and perform cryptographic operations. Keys stored in the TPM can't be extracted, even by the operating system.

### Secure Enclave
Apple's equivalent of TPM, found in iPhones, iPads, and Macs. A separate processor dedicated to security operations.

### StrongBox
Android's hardware security module, found in newer Android devices. Provides similar capabilities to TPM and Secure Enclave.

### App Sandbox
Operating system feature that isolates applications from each other. Each app runs in its own restricted environment with limited access to system resources.

---

## Common Abbreviations

**AES** — Advanced Encryption Standard (the encryption algorithm)

**BIP** — Bitcoin Improvement Proposal (standards for Bitcoin wallets)

**NIST** — National Institute of Standards and Technology (US standards body)

**PQ** — Post-Quantum (cryptography designed for quantum computers)

**MPC** — Multi-Party Computation (key splitting technology)

**HSM** — Hardware Security Module (security chip)

**IPC** — Inter-Process Communication (how components talk to each other)

---

## Messaging & Chat Terms

### MLS (Messaging Layer Security)
A cryptographic protocol standardized by the IETF for secure group messaging. It ensures that messages can't be tampered with and only intended recipients can read them. Zbelthas uses MLS for all group conversations.

### Perfect Forward Secrecy
A property where compromising one encryption key doesn't compromise past or future messages. Zbelthas generates a new key for every message, so even if an attacker gets one key, they can only decrypt that single message.

### CRDT (Conflict-free Replicated Data Type)
A data structure that allows multiple devices to sync without a central server. Your messages sync across all your devices automatically, even if you're offline when they arrive.

### ML-KEM-768
The post-quantum key exchange algorithm Zbelthas uses for chat. It protects your conversations against future quantum computers.

### Peer-to-Peer (P2P)
Direct communication between devices without a central server. Your messages go straight from your device to the recipient's device—no one in between.

### libp2p
A battle-tested peer-to-peer networking library. Zbelthas uses it to establish direct connections between users for chat and video calls.

### IPFS (InterPlanetary File System)
A decentralized file storage network. Zbelthas uses it to store voice messages and files temporarily, encrypted so the network can't read them.

### SRTP (Secure Real-time Transport Protocol)
Encryption for voice and video calls. Zbelthas uses SRTP with AES-256-GCM to protect your calls.

### Disappearing Messages
Messages that automatically delete after a specified time (5 seconds to 7 days). When they're deleted, they're securely erased from all devices—not just hidden.

---

## Browser & Privacy Terms

### Zero Persistent Storage
The browser doesn't save anything—no cookies, no history, no cache. When you close the browser, everything is erased. This isn't just clearing history; it's running in a mode where nothing is saved in the first place.

### Fingerprint Randomization
Websites identify you by your "browser fingerprint"—a combination of screen size, fonts, timezone, and other characteristics. Zbelthas randomizes these characteristics every session, making you look like a different person each time.

### DNS-over-HTTPS (DoH)
Encrypting DNS queries so your ISP can't see which websites you visit. Normally, DNS requests are unencrypted, allowing ISPs to track your browsing.

### Content Security Policy (CSP)
Rules that control what a web page can do. Zbelthas enforces strict CSP to block JavaScript execution, inline scripts, and other common attack vectors.

### WebView
The component that renders web pages. Zbelthas uses platform-specific WebView technology (WebView2 on Windows, WKWebView on Apple, Android WebView) running in a separate isolated process.

### dApp (Decentralized Application)
A web application that interacts with blockchains. Zbelthas Browser lets you use dApps securely through native wallet integration.

### Native Confirmation Popup
When a dApp wants to sign a transaction, Zbelthas shows a confirmation in native UI (not web content). This prevents malicious websites from faking transaction details.

---

## Worker & Architecture Terms

### Worker
An isolated process that handles a specific function. Zbelthas has four workers: Wallet, Messaging, Browser, and P2P. Each runs in its own sandbox.

### Supervisor
The security checkpoint that mediates between workers. All communication flows through the Supervisor, which verifies every request and enforces security policy.

### Physical Separation
Workers don't link against each other's code. If the Browser Worker is compromised, the attacker can't access wallet functions because those functions don't exist in the browser binary.

### Deaf Architecture
The Wallet Worker only accepts commands from the Supervisor and ignores everything else. It can't be contacted directly by other workers or the host.

---

## Learn More

For detailed explanations of how these concepts work together in Zbelthas, see the other whitepapers:

- **Overview and Vision** — The big picture
- **System Architecture** — How components work together
- **Cryptographic Foundations** — The mathematics of protection
- **Security Features** — Eight layers of defense
- **Platform Features** — Wallet, Chat, and Browser
- **Legal & Compliance** — Regulatory implications
- **Chat & Messaging** — Secure communication
- **Browser & Web3** — Privacy browsing

---
Title: Zbelthas - Glossary
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.



# Zbelthas™ Whitepaper Suite

## Understanding the Future of Digital Asset Security

---

## Table of Contents

- [Welcome](#welcome)
- [Executive Summary](#executive-summary)
- [The Documents](#the-documents)
- [How to Read These Documents](#how-to-read-these-documents)
- [What Makes Zbelthas Different](#what-makes-zbelthas-different)
- [What We Are Not](#what-we-are-not)
- [Our Commitment to Transparency](#our-commitment-to-transparency)
- [Timeline](#timeline)
- [A Note on Security](#a-note-on-security)
- [Support the Project](#support-the-project)

---

## Welcome

You're holding the documentation for Zbelthas—a new approach to protecting your digital assets. These whitepapers explain not just what Zbelthas does, but why we built it the way we did.

We believe security shouldn't require a PhD to understand. These documents are written for curious people who want to know how their assets are protected, not just that they're protected.

---

## Executive Summary

**Short on time?** Start with our [Executive Summary](00_EXECUTIVE_SUMMARY.md) — a two-page overview of everything Zbelthas offers.

---

## The Documents

This suite consists of eight whitepapers plus a glossary, each exploring a different aspect of Zbelthas. You can read them in any order, though we recommend starting with the Overview if you're new to Zbelthas.

### [1. Overview and Vision](01_OVERVIEW_AND_VISION.md)

**Start here.** This document explains why Zbelthas exists, what problems it solves, and how it's different from other solutions. You'll learn about the quantum computing threat, our three-module platform (Wallet, Chat, Browser), and our development roadmap.

*Reading time: 15-20 minutes*

---

### [2. System Architecture](02_ARCHITECTURE.md)

How Zbelthas is built. This document explains our zero-trust architecture with four isolated workers (Wallet, Messaging, Browser, P2P) and the Supervisor that mediates between them. Think of it as understanding how a secure building is designed, with different zones, access controls, and security checkpoints.

*Reading time: 15-20 minutes*

---

### [3. Cryptographic Foundations](03_CRYPTOGRAPHY.md)

The mathematics protecting your data. We explain post-quantum cryptography, key splitting, and memory protection in terms anyone can understand. You'll learn why these technologies matter for wallet security, chat encryption, and browser privacy.

*Reading time: 20-25 minutes*

---

### [4. Security Features](04_SECURITY_FEATURES.md)

Eight layers of defense. Like a medieval castle with multiple walls, Zbelthas implements independent security layers that protect all three modules. This document explains each layer and why defense in depth matters.

*Reading time: 15-20 minutes*

---

### [5. Platform Features](05_PLATFORM_FEATURES.md)

The complete platform. This document provides an overview of all three modules—Wallet, Chat, and Browser—and explains how they work together while remaining isolated for security.

*Reading time: 15-20 minutes*

---

### [6. Legal & Compliance](06_LEGAL_AND_COMPLIANCE.md)

Privacy and regulation. Our non-custodial, serverless architecture has profound legal implications. This document explains what that means for your rights, your privacy, and your responsibilities across wallet, chat, and browser usage.

*Reading time: 15-20 minutes*

---

### [7. Chat & Messaging](07_CHAT_AND_MESSAGING.md)

Secure communication in depth. This document explores the chat module in detail: MLS encryption, peer-to-peer architecture, voice messages, video calls, file sharing, disappearing messages, and group conversations. Learn why serverless messaging provides privacy that traditional apps cannot.

*Reading time: 15-20 minutes*

---

### [8. Browser & Web3](08_BROWSER_AND_WEB3.md)

Privacy browsing and Web3 integration. This document explores the browser module: zero persistent storage, fingerprint randomization, encrypted DNS, Web3 dApp interaction, and the security isolation that protects your wallet from malicious websites.

*Reading time: 15-20 minutes*

---

### [9. Wallet Details](09_WALLET_DETAILS.md)

Multi-chain cryptocurrency management. This document provides complete details on the wallet module: supported blockchains, non-custodial architecture, key protection, sending and receiving, backup and recovery, NFT support, and advanced features. Learn how your crypto is protected with hardware-backed security and post-quantum cryptography.

*Reading time: 20-25 minutes*

---

### [Glossary](GLOSSARY.md)

Terms and concepts. A reference guide explaining the terminology used throughout these documents, written in plain language.

---

## How to Read These Documents

### If You're New to Crypto Security

Start with the **Overview and Vision**, then read **Security Features** to understand the layers of protection. The **Wallet & Blockchain** document will help you understand practical usage.

### If You're Evaluating Zbelthas

Read the **Overview and Vision** for the big picture, then **Legal & Compliance** to understand the regulatory implications. The **Architecture** document explains how we achieve our security claims.

### If You're Technically Curious

The **Cryptographic Foundations** document goes deepest into the mathematics and algorithms. **Architecture** explains the system design, and **Security Features** covers the implementation details.

### If You're Concerned About Privacy

Start with **Legal & Compliance** to understand our zero-data-collection architecture. The **Architecture** document explains how this is technically enforced.

---

## What Makes Zbelthas Different

**Non-Custodial:** We don't hold your keys. We can't freeze your assets, comply with seizure orders, or lose your funds in a hack. You maintain complete control.

**Post-Quantum Ready:** We use cryptography designed to resist both today's computers and tomorrow's quantum computers. Your assets are protected against threats that don't exist yet.

**Zero Data Collection:** We don't collect personal information, transaction history, or usage analytics. There's no database to breach, no data to sell, no logs to subpoena.

**Defense in Depth:** Eight independent security layers protect your assets. Even if an attacker defeats one layer, seven more stand in their way.

**Hardware Security Integration:** We leverage the security chips built into modern devices—TPM, Secure Enclave, StrongBox—to provide hardware-level protection without requiring separate hardware.

---

## Our Commitment to Transparency

These whitepapers represent our commitment to transparency. We believe you have the right to understand how your security works, not just trust that it does.

We've written these documents to be accessible without sacrificing accuracy. Where we've simplified, we've done so carefully. Where technical precision matters, we've preserved it.

If you have questions these documents don't answer, we want to hear from you. Security through obscurity isn't security at all.

---

## Timeline

**April 2025:** Development begins  
**Q2-Q3 2025:** Core security architecture  
**Q4 2025:** Multi-platform development  
**Q1 2026:** Testing and refinement  
**March 2026:** Private release  
**2026 and beyond:** Continuous improvement  

---

## What We Are Not

**Zbelthas is software — we do not issue, sell, or manage any cryptocurrency, token, or digital asset.**

- We are **not** a cryptocurrency or token
- We are **not** an exchange or trading platform
- We are **not** a custodian or financial service
- We are **not** an investment product

We build security software. You use it to protect assets you already own.

---

## A Note on Security

No security system is perfect. We're transparent about what Zbelthas can and cannot protect against. We protect against remote attacks, malware, memory forensics, and future quantum computers. We cannot fully protect against physical access to an unlocked device or user error.

Security is a partnership. We provide the strongest protection possible; you need to protect your device and your recovery phrase.

---

## Support the Project

Zbelthas is built by a small team committed to real security and privacy. If you believe in what we're building, you can support our development.

**Traditional Methods:** Visit [zbelthas.com/donate](https://zbelthas.com/donate) for Patreon and other payment options.

**Web3 / Cryptocurrency:** For on-chain donations, visit our Web3 portal at [rpc.zbelthas.com](https://rpc.zbelthas.com) where you can view and interact with our donation smart contract. The contract only receives donations—no tokens are issued, no rewards are promised.

*Donations do not grant any rights, tokens, equity, or promises of future benefits.*

---
Title: Zbelthas Whitepaper Suite
Version: 2.0
Date: March 2026
Status: Public Whitepaper
Copyright: © 2026 Zbelthas Project. All rights reserved.
Trademark: Zbelthas™ is a registered trademark.

