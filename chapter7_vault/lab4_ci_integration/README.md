
---

## 📘 Lab 4 — CI Integration

```bash
cat >> chapter7_vault/lab4_ci_integration/README.md << 'EOF'
# Lab 4: Vault CI Integration

## Objective
Integrate Vault secrets into CI/CD pipeline.

## Prerequisites
- Drone CI installed
- Vault running

## Steps
1. Store secret in Vault.
2. Fetch secret in pipeline.
3. Use secret in build.

## Commands
```yaml
- name: use-secret
  image: alpine
  commands:
    - export SECRET=$(vault kv get -field=value secret/api)
    - echo $SECRET
