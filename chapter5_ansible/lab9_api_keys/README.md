
# Lab 9: API Keys Management

## Objective
Manage API keys securely with Ansible.

## Prerequisites
- Ansible installed
- Vault configured

## Steps
1. Store API key in Vault.
2. Inject into playbook.
3. Use in application config.

## Commands
```yaml
- hosts: servers
  tasks:
    - name: Configure API key
      copy:
        content: "{{ lookup('ansible.builtin.vault', 'api_key') }}"
        dest: /etc/app/api_key.txt
