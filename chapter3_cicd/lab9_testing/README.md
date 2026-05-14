
---

## 📘 Lab 9 — Testing Pipeline

```markdown
# Lab 9: Testing Pipeline

## Objective
Run automated tests in Drone CI.

## Prerequisites
- Test suite available in repo

## Steps
1. Add test stage in `.drone.yml`.
2. Run unit tests automatically.

## Commands
```yaml
- name: unit-tests
  image: node:18
  commands:
    - npm install
    - npm test
