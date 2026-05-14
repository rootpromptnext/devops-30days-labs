# Lab 2: CI/CD Pipeline

## Objective
Configure Drone CI pipeline for the capstone project.

## Prerequisites
- Drone CI installed
- Repo connected

## Steps
1. Create `.drone.yml`.
2. Add build + test stages.
3. Push to repo.

## Commands
```yaml
kind: pipeline
type: docker
name: capstone

steps:
- name: build
  image: node:18
  commands:
    - npm install
    - npm run build

- name: test
  image: node:18
  commands:
    - npm test
