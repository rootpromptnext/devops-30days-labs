
---

## 📘 Lab 3 — Cross‑Sprint Collaboration (Measurement)

```markdown
# Lab 3: Cross-Sprint Collaboration

## Objective
Measure collaboration across sprints using commit activity.

## Prerequisites
- Gitea repo with multiple contributors

## Steps
1. Each team member commits to `dev` branch.
2. Use `git shortlog` to measure contributions.
3. Export commit stats to CSV.

## Commands
```bash
git shortlog -s -n > sprint1_commits.txt
