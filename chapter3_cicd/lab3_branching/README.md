# Lab 3: Branching Strategy

## Objective
Implement Git branching for feature development.

## Prerequisites
- Repo created in Gitea

## Steps
1. Create `feature/login` branch.
2. Add login code.
3. Merge into `main`.

## Commands
```bash
git checkout -b feature/login
echo "Login feature code" > login.txt
git add login.txt
git commit -m "Add login feature"
git checkout main
git merge feature/login
git push origin main
```
