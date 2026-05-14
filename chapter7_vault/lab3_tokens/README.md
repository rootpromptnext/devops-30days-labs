
# Lab 3: Vault Tokens

## Objective
Generate and manage Vault tokens.

## Prerequisites
- Vault running

## Steps
1. Create token.
2. List tokens.
3. Revoke token.

## Commands
```bash
vault token create -policy=readonly
vault list auth/token/accessors
vault token revoke <token_id>
```
