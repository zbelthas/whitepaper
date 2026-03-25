

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

