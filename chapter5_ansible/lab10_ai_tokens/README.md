
---

## 📘 Lab 10 — AI Tokens Management

```markdown
# Lab 10: AI Tokens Management

## Objective
Manage ML/AI tokens securely with Ansible.

## Prerequisites
- Ansible installed
- Vault configured

## Steps
1. Store ML token in Vault.
2. Inject into ML pipeline config.
3. Run pipeline.

## Commands
```yaml
- hosts: servers
  tasks:
    - name: Configure ML token
      copy:
        content: "{{ lookup('ansible.builtin.vault', 'ml_token') }}"
        dest: /etc/ml/token.txt
