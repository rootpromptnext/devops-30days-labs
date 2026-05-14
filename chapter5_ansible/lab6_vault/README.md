
---

## 📘 Lab 6 — Ansible Vault

```markdown
# Lab 6: Ansible Vault

## Objective
Encrypt sensitive data using Ansible Vault.

## Prerequisites
- Ansible installed

## Steps
1. Create secrets file.
2. Encrypt file.
3. Use in playbook.

## Commands
```bash
ansible-vault create secrets.yml
ansible-vault encrypt secrets.yml
ansible-playbook -i inventory.ini playbook.yml --ask-vault-pass
