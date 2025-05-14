# 🧠 BrainSAIT Tailscale Control

This repository manages and synchronizes the **Tailscale ACLs** that govern access across the secure, multi-cloud **BrainSAIT Agentic Infrastructure**.

All changes to access control are tracked in Git, reviewed, and deployed automatically via GitHub Actions — empowering a **GitOps-driven security model**.

---

## 🔐 What This Repo Does

- 📡 **Controls machine-to-machine access** in the Tailscale mesh
- 🔒 **Defines SSH and subnet access** between Mac, Windows, Pi, Arduino, and cloud nodes
- 🔁 **Automatically syncs ACLs** to Tailscale when commits are pushed to `main`
- ✅ **Enables auditability and rollback** of network policy changes

---

## 📂 Repository Structure

```plaintext
.
├── tailscale/
│   └── acls.json           # All ACL rules, device tags, groups, routes
└── .github/
    └── workflows/
        └── sync-acl.yml    # GitHub Actions workflow for automatic ACL deployment
