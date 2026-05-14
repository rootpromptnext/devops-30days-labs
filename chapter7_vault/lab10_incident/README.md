# Lab 10: Incident Handling with Vault

## Objective
Respond to secret compromise incidents using Vault.

## Prerequisites
- Vault running

## Steps
1. Revoke compromised token.
2. Rotate affected secrets.
3. Document incident.

## Commands
```bash
vault token revoke <compromised_token>
vault kv delete secret/db
vault kv put secret/db password=newsecret
