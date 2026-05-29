# 🔐 Me2em Organization

> **One cryptographic Identity → unlimited isolated Handles → contextual Sessions**

[![Website](https://img.shields.io/badge/website-me2em.com-blue)](https://me2em.com)
[![Docs](https://img.shields.io/badge/docs-docs.me2em.com-blue)](https://docs.me2em.com)
[![npm](https://img.shields.io/badge/npm-@me2em-red)](https://www.npmjs.com/org/me2em)
[![License](https://img.shields.io/badge/license-Apache--2.0-green)](https://github.com/me2em-org/me2em-protocol/blob/main/LICENSE)

---

## 🎯 What is Me2em?

Me2em is an **open authorization protocol** that redefines digital identity for the privacy-first era.

### Traditional auth forces:
```
One User = One Profile
```
❌ Your boss sees your dating profile  
❌ Your IoT devices share credentials with your personal account  
❌ You must reveal email/phone to every new app  

### Me2em enables:
```
One Identity → Unlimited Handles → Contextual Sessions
```
✅ `@alice_work`, `@alice_private`, `@alice_iot` — all from one seed phrase  
✅ Granular access: compromise one Handle, not your entire identity  
✅ Apps receive only a public Handle — no email, no phone, no tracking  

---

## 🗂️ Ecosystem Map

| Repository | Description | Status | Language |
|------------|-------------|--------|----------|
| [`me2em-protocol`](https://github.com/me2em-org/me2em-protocol) | Core spec + reference implementation (NestJS) | 🟢 Active | TypeScript |
| [`leteem`](https://github.com/me2em-org/leteem) | E2EE messenger using Me2em auth | 🟡 Beta | TypeScript + React |
| [`sdk-js`](https://github.com/me2em-org/sdk-js) | TypeScript SDK for web/mobile | 🟡 Planned | TypeScript |
| [`sdk-rust`](https://github.com/me2em-org/sdk-rust) | Rust SDK for embedded/IoT | ⚪ Roadmap | Rust |
| [`website`](https://github.com/me2em-org/website) | Landing + documentation (Astro) | 🟡 Planned | Astro + React |
| [`.github`](https://github.com/me2em-org/.github) | Shared templates, workflows, governance | 🟢 Active | Markdown |

> 💡 **Tip**: Click any repository to explore code, issues, and contribution guides.

---

## 🚀 Get Started

### For Developers
```bash
# Install the core SDK
npm install @me2em/protocol-core

# Quick example
import { Identity } from '@me2em/protocol-core';
const identity = await Identity.fromSeed('your-seed-phrase');
const handle = await identity.deriveHandle('work');
```

### For Self-Hosting
```bash
git clone https://github.com/me2em-org/me2em-protocol.git
cd me2em-protocol
docker compose up -d
```
📖 Full guide: [`docs/SELF_HOSTING.md`](https://github.com/me2em-org/me2em-protocol/blob/main/docs/SELF_HOSTING.md)

### For Documentation
📘 Protocol spec, SDK reference, tutorials:  
→ [docs.me2em.com](https://docs.me2em.com)

---

## 🤝 Contributing

We welcome contributors of all skill levels!

### Start here:
- 🐛 [Good first issues](https://github.com/me2em-org/me2em-protocol/issues?q=label:good-first-issue)
- 📝 [Documentation improvements](https://github.com/me2em-org/me2em-protocol/issues?q=label:documentation)
- 💡 [Propose a feature](https://github.com/me2em-org/me2em-protocol/discussions)

### Resources:
- [CONTRIBUTING.md](https://github.com/me2em-org/me2em-protocol/blob/main/CONTRIBUTING.md) — How to contribute
- [GOVERNANCE.md](https://github.com/me2em-org/me2em-protocol/blob/main/GOVERNANCE.md) — How decisions are made
- [CODE_OF_CONDUCT.md](https://github.com/me2em-org/me2em-protocol/blob/main/CODE_OF_CONDUCT.md) — Community guidelines

### Become a Maintainer
Active contributors may be invited to join the core team. See [GOVERNANCE.md](https://github.com/me2em-org/me2em-protocol/blob/main/GOVERNANCE.md) for criteria.

---

## 🔐 Security

Me2em handles cryptographic identities. Security is our top priority.

### Reporting a vulnerability:
1. **Do NOT** open a public issue
2. Email `security@me2em.com` with details
3. We respond within 72 hours

📋 Full policy: [SECURITY.md](https://github.com/me2em-org/me2em-protocol/blob/main/SECURITY.md)

### Best practices for implementers:
- Store seed phrases in secure, user-controlled storage
- Use short-lived sessions and rotate tokens
- Validate Handle metadata server-side
- Keep `@me2em/*` packages updated

---

## 📡 Stay Connected

| Channel | Link |
|---------|------|
| 🌐 Website | [me2em.com](https://me2em.com) |
| 📚 Documentation | [docs.me2em.com](https://docs.me2em.com) |
| 📦 npm packages | [`@me2em`](https://www.npmjs.com/org/me2em) |
| 💬 Discussions | [GitHub Discussions](https://github.com/me2em-org/me2em-protocol/discussions) |
| 📧 Contact | `hello@me2em.com` |
| 🔐 Security | `security@me2em.com` |

---

## 📜 License

All core Me2em projects are licensed under [Apache License 2.0](https://github.com/me2em-org/me2em-protocol/blob/main/LICENSE), unless otherwise noted.

© 2026 Me2em Organization. Built with ❤️ for privacy, openness, and user sovereignty.