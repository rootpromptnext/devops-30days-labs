# Lab 1: Capstone Repo Setup

## Objective
Initialize Git repository for the capstone project.

## Prerequisites
- Gitea running
- Git installed

## Steps
1. Create repo `capstone-ecommerce`.
2. Clone locally.
3. Add initial README.

## Commands
```bash
git clone ssh://gitea@localhost:222/capstone-ecommerce.git
cd capstone-ecommerce
echo "# Capstone E-Commerce Project" > README.md
git add .
git commit -m "Initial commit"
git push origin main
