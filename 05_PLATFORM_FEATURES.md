

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
