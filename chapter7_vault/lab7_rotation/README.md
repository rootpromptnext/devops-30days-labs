# Lab 7: Secrets Rotation

## Objective
Rotate secrets automatically using Vault.

## Prerequisites
- Vault running

## Steps
1. Enable database secrets engine.
2. Configure rotation policy.
3. Verify rotated credentials.

## Commands
```bash
vault secrets enable database
vault write database/config/mydb \
  plugin_name=postgresql-database-plugin \
  allowed_roles="readonly" \
  connection_url="postgresql://user:pass@localhost:5432/"
vault write database/roles/readonly \
  db_name=mydb \
  creation_statements="CREATE ROLE \"{{name}}\" WITH LOGIN PASSWORD '{{password}}';"
