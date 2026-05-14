# Lab 6: Loki Setup

## Objective
Install Loki for log aggregation.

## Prerequisites
- Kubernetes cluster
- Helm installed

## Steps
1. Add Loki Helm repo.
2. Install Loki.
3. Verify pods.

## Commands
```bash
helm repo add grafana https://grafana.github.io/helm-charts
helm install loki grafana/loki-stack
kubectl get pods -n default
