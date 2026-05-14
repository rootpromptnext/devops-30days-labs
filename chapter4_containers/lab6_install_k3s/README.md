# Lab 6: Install K3s

## Objective
Set up a lightweight Kubernetes cluster.

## Prerequisites
- Linux VM
- Root access

## Steps
1. Install K3s via script.
2. Verify cluster status.

## Commands
```bash
curl -sfL https://get.k3s.io | sh -
sudo kubectl get nodes
```
