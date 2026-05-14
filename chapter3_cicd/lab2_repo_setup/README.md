
---

## 📘 Lab 2 — Repo Setup

```markdown
# Lab 2: Repo Setup in Gitea

## Objective
Create a repository and push code to Gitea.

## Prerequisites
- Gitea running
- Git installed locally

## Steps
1. Create repo `ecommerce-app` in Gitea.
2. Clone repo locally.
3. Add a sample file and push.

## Commands
```bash
git clone ssh://gitea@localhost:222/ecommerce-app.git
cd ecommerce-app
echo "# E-Commerce App" > README.md
git add .
git commit -m "Initial commit"
git push origin main
