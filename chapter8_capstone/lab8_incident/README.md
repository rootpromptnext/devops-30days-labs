# Lab 8: Incident Simulation

## Objective
Simulate and respond to an outage.

## Prerequisites
- Monitoring + logging enabled

## Steps
1. Kill app pod.
2. Observe alert.
3. Restore pod.

## Commands
```bash
kubectl delete pod <pod_name>
kubectl rollout restart deployment capstone-app
```
