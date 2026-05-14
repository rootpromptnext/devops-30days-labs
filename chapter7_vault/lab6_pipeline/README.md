# Lab 6: Pipeline Secrets

## Objective
Inject secrets from Vault into CI/CD pipelines.

## Prerequisites
- Vault running
- Drone CI configured

## Steps
1. Store secret in Vault KV.
2. Configure Drone pipeline to fetch secret.
3. Use secret in build stage.

## Commands
```bash
vault kv put secret/db password=supersecret
> - name: db-connection
  image: alpine
  commands:
    - export DB_PASS=$(vault kv get -field=password secret/db)
    - echo "Connecting with $DB_PASS"
