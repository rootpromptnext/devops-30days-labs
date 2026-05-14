# Lab 10: Deployment Pipeline

## Objective
Deploy application automatically after tests pass.

## Prerequisites
- K3s cluster running
- Drone CI configured

## Steps
1. Add deployment stage in `.drone.yml`.
2. Apply Kubernetes manifests.

## Commands
```yaml
- name: deploy
  image: bitnami/kubectl
  settings:
    manifests:
      - k8s/deployment.yaml
      - k8s/service.yaml
```
