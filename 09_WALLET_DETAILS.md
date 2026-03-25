

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

