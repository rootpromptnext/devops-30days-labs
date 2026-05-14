# Lab 9: ML Pipeline Secrets

## Objective
Secure ML pipeline tokens with Vault.

## Prerequisites
- ML pipeline configured
- Vault running

## Steps
1. Store ML token in Vault.
2. Fetch token in pipeline.
3. Use token for model API.

## Commands
```bash
vault kv put secret/ml token=abcd1234
- name: ml-job
  image: python:3.9
  commands:
    - export ML_TOKEN=$(vault kv get -field=token secret/ml)
    - python run_pipeline.py --token $ML_TOKEN
