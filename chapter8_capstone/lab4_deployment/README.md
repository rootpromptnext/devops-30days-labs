# Lab 4: Deployment on K3s

## Objective
Deploy the containerized app on K3s.

## Prerequisites
- K3s cluster running
- kubectl configured

## Steps
1. Create deployment manifest.
2. Apply manifest.
3. Verify pods.

## Commands
```bash
kubectl apply -f deployment.yaml
kubectl get pods
