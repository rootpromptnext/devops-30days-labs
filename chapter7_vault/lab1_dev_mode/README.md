# Lab 1: Vault Dev Mode

## Objective
Run HashiCorp Vault in dev mode for quick testing.

## Prerequisites
- Linux VM
- Vault installed

## Steps
1. Start Vault in dev mode.
2. Export root token.
3. Verify status.

## Commands
```bash
vault server -dev
export VAULT_ADDR='http://127.0.0.1:8200'
export VAULT_TOKEN='root'
vault status


# Lab 1: Vault Dev Mode

## Objective
Run HashiCorp Vault in dev mode for quick testing.

## Prerequisites
- Linux VM
- Vault installed

## Steps
1. Start Vault in dev mode.
2. Export root token.
3. Verify status.

## Commands
```bash
vault server -dev
export VAULT_ADDR='http://127.0.0.1:8200'
export VAULT_TOKEN='root'
vault status
```
