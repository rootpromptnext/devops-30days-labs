# Lab 5: Vault Audit Logs

## Objective
Enable and review Vault audit logs.

## Prerequisites
- Vault running

## Steps
1. Enable audit device.
2. Perform secret operations.
3. Review logs.

## Commands
```bash
vault audit enable file file_path=/var/log/vault_audit.log
vault kv put secret/demo value=123
cat /var/log/vault_audit.log
