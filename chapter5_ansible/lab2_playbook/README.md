
# Lab 2: Playbook Basics

## Objective
Write and run your first Ansible playbook.

## Prerequisites
- Ansible installed
- Inventory file ready

## Steps
1. Create playbook to install Nginx.
2. Run playbook.
3. Verify service.

## Commands
```yaml
# playbook.yml
- hosts: servers
  tasks:
    - name: Install Nginx
      apt:
        name: nginx
        state: present
```
