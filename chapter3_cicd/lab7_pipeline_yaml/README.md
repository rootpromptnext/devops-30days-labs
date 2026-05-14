
---

## 📘 Lab 7 — Pipeline YAML

```markdown
# Lab 7: Drone CI Pipeline YAML

## Objective
Define a CI/CD pipeline in `.drone.yml`.

## Prerequisites
- Drone CI installed
- Repo connected to Drone

## Steps
1. Create `.drone.yml` in repo root.
2. Add build + test stages.
3. Commit and push.

## Commands
```yaml
kind: pipeline
type: docker
name: default

steps:
- name: build
  image: golang
  commands:
    - go build

- name: test
  image: golang
  commands:
    - go test ./...
