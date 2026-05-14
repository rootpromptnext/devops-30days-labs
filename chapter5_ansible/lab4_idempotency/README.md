
---

## 📘 Lab 4 — Idempotency

```markdown
# Lab 4: Idempotency

## Objective
Demonstrate idempotency in Ansible tasks.

## Prerequisites
- Ansible installed

## Steps
1. Run playbook twice.
2. Observe that second run makes no changes.

## Commands
```yaml
- hosts: servers
  tasks:
    - name: Ensure Nginx is installed
      apt:
        name: nginx
        state: present
