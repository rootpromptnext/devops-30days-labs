
---

## 📘 Lab 8 — Scaling Pods

```markdown
# Lab 8: Scaling Pods

## Objective
Scale application replicas in K3s.

## Prerequisites
- App deployed on K3s

## Steps
1. Scale deployment.
2. Verify replicas.

## Commands
```bash
kubectl scale deployment myapp --replicas=3
kubectl get pods
