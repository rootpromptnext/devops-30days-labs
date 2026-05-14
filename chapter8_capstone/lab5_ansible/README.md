# Lab 5: Ansible Automation

## Objective
Automate infrastructure setup with Ansible.

## Prerequisites
- Ansible installed
- Inventory file ready

## Steps
1. Write playbook for app deployment.
2. Run playbook.
3. Verify deployment.

## Commands
```yaml
- hosts: servers
  tasks:
    - name: Deploy app
      kubernetes.core.k8s:
        state: present
        definition: "{{ lookup('file', 'deployment.yaml') }}"
