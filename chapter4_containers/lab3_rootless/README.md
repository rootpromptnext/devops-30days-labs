
---

## 📘 Lab 3 — Rootless Containers

```markdown
# Lab 3: Rootless Containers

## Objective
Run Podman containers without root privileges.

## Prerequisites
- Podman installed
- Non‑root user account

## Steps
1. Configure user namespaces.
2. Run container as non‑root.
3. Verify isolation.

## Commands
```bash
podman run --userns=keep-id alpine whoami
