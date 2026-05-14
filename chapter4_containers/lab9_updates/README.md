
---

## 📘 Lab 9 — Rolling Updates

```markdown
# Lab 9: Rolling Updates

## Objective
Perform rolling updates in K3s.

## Prerequisites
- Deployment running

## Steps
1. Update image version.
2. Apply manifest.
3. Observe rollout.

## Commands
```bash
kubectl set image deployment/myapp myapp=myapp:2.0
kubectl rollout status deployment/myapp
