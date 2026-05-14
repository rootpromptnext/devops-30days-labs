# Lab 1: Ansible Setup

## Objective
Install and configure Ansible for infrastructure automation.

## Prerequisites
- Linux VM
- Python installed

## Steps
1. Install Ansible.
2. Verify installation.
3. Create inventory file.

## Commands
```bash
sudo apt update && sudo apt install ansible -y
ansible --version
echo "[servers]" > inventory.ini
echo "localhost ansible_connection=local" >> inventory.ini
