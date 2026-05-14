
# Lab 8: Secure Pipeline

## Objective
Integrate Ansible with CI/CD securely.

## Prerequisites
- Drone CI installed
- Ansible playbook ready

## Steps
1. Add Ansible stage in `.drone.yml`.
2. Use Vault for secrets.
3. Deploy infra via pipeline.

## Commands
```yaml
- name: ansible-deploy
  image: ansible/ansible-runner
  commands:
    - ansible-playbook -i inventory.ini site.yml --vault-password-file .vault_pass
