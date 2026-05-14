
# Lab 10: Model Serving in K3s

## Objective
Deploy ML model as a service in K3s.

## Prerequisites
- K3s cluster
- Containerized ML model

## Steps
1. Create deployment for ML model.
2. Expose service.
3. Test inference endpoint.

## Commands
```bash
kubectl apply -f ml-deployment.yaml
kubectl apply -f ml-service.yaml
curl http://<node-ip>:<port>/predict
