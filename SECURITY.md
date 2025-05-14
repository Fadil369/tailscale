# Security Policy

## 🔐 Reporting a Vulnerability

If you believe you have found a security vulnerability in this repository or any related BrainSAIT system:

- Please **DO NOT open an issue or pull request.**
- Instead, email us directly at: **security@brainsait.io**
- You may also use GPG encryption (key fingerprint and details available upon request).

We take all reports seriously and will respond as quickly as possible.

---

## 📆 Supported Versions

| Version Branch | Supported | Notes                |
|----------------|-----------|----------------------|
| `main`         | ✅        | Production ACL sync  |
| `dev`          | ✅        | Actively developed   |
| others         | ❌        | Not maintained       |

---

## 🛡️ Security Best Practices

This repository manages **ACLs for the BrainSAIT Tailscale network** and adheres to the following principles:

- ✅ GitOps-based change control
- ✅ API keys are stored as GitHub Secrets
- ✅ All ACL changes are reviewed and validated before deployment
- ✅ Changes are applied only on `main` or approved pull requests

---

## 🔏 Disclosure Process

1. Submit the report privately to **security@brainsait.io**
2. We will acknowledge receipt within **48 hours**
3. A timeline for resolution will be provided, typically within **7 days**
4. Coordinated disclosure and public advisories will follow when appropriate

---

## 🔐 Tailscale ACL Context

This repo controls:

- Tailscale access rules for `brainsait.io`, `brainsait.uk`, and `thefadil.site` tailnets
- SSH access between trusted machines
- Routing rules and subnet exposure

Modifying ACLs here may affect **real-time infrastructure access**. Please review all commits with care.

---

_Authored by **Dr. Mohamed El Fadil** — BRAINSAIT Founder & Security Lead_
