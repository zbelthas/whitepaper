

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

