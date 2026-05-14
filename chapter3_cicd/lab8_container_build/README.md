# Lab 8: Container Build with Drone CI

## Objective
Build container images automatically in CI.

## Prerequisites
- Podman installed
- Drone CI pipeline configured

## Steps
1. Add container build step in `.drone.yml`.
2. Push image to local registry.

## Commands
```yaml
- name: container-build
  image: plugins/podman
  settings:
    repo: localhost:5000/ecommerce-app
    tags: latest
```
