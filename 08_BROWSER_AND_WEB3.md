

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

