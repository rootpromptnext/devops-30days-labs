# Lab 8: Vault + Kubernetes Integration

## Objective
Inject secrets into Kubernetes pods using Vault.

## Prerequisites
- K3s cluster
- Vault running

## Steps
1. Enable Kubernetes auth in Vault.
2. Configure role binding.
3. Deploy pod with Vault sidecar.

## Commands
```bash
vault auth enable kubernetes
vault write auth/kubernetes/role/demo \
  bound_service_account_names=demo-sa \
  bound_service_account_namespaces=default \
  policies=readonly \
  ttl=1h
