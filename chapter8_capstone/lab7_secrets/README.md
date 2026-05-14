# Lab 7: Secrets Management

## Objective
Secure app secrets with Vault.

## Prerequisites
- Vault running

## Steps
1. Store DB password in Vault.
2. Inject secret into app.
3. Verify secure access.

## Commands
```bash
vault kv put secret/db password=supersecret
```
