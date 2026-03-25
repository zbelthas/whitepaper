

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

