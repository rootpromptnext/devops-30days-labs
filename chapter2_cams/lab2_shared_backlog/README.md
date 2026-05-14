
---

## 📘 Lab 2 — Shared Backlog (Automation)

```markdown
# Lab 2: Shared Backlog Automation

## Objective
Automate backlog management using Git issues.

## Prerequisites
- Gitea running locally
- Repo created

## Steps
1. Enable issue tracking in Gitea.
2. Create issues for features, bugs, and tasks.
3. Automate labeling with Drone CI:
   - Add `.drone.yml` to auto‑tag commits with issue IDs.

## Commands
```yaml
# .drone.yml snippet
pipeline:
  label-issues:
    image: alpine/git
    commands:
      - git log --oneline | grep ISSUE-
