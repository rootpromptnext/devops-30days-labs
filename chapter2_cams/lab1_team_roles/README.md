# Lab 1: Team Roles & Collaboration

## Objective
Practice collaboration by defining clear DevOps roles in a project.

## Prerequisites
- Git installed
- Local repo initialized (`git init`)

## Steps
1. Create a new repo in Gitea called `team-collab`.
2. Add three branches: `dev`, `qa`, `prod`.
3. Assign roles:
   - Developer → pushes to `dev`
   - QA → merges into `qa`
   - Ops → deploys from `prod`
4. Document responsibilities in `README.md`.

## Commands
```bash
git checkout -b dev
git checkout -b qa
git checkout -b prod
