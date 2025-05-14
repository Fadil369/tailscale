---
title: Usage
---

# ⚙️ ACL Usage Guide

Edit your ACLs in `tailscale/acls.json`, using the following structure:

```json
{
  "tagOwners": {
    "tag:macbook": ["user:fadil369@github"]
  },
  "acls": [
    {
      "action": "accept",
      "src": ["tag:macbook"],
      "dst": ["tag:win10:*"]
    }
  ]
}