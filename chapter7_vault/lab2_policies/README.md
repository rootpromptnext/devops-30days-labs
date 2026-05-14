# Lab 2: Vault Policies

## Objective
Create and apply Vault policies.

## Prerequisites
- Vault running

## Steps
1. Write policy file.
2. Apply policy.
3. Assign to token.

## Commands

cat > readonly.hcl <<EOF
path "secret/*" {
  capabilities = ["read"]
}
EOF

vault policy write readonly readonly.hcl
vault token create -policy=readonly
