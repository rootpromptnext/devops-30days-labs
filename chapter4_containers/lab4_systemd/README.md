# Lab 4: Podman + Systemd

## Objective
Manage containers as systemd services.

## Prerequisites
- Podman installed
- Systemd available

## Steps
1. Generate systemd unit file.
2. Enable service.
3. Verify container auto‑starts.

## Commands
```bash
podman generate systemd --name myapp > myapp.service
sudo systemctl enable myapp.service
sudo systemctl start myapp.service
```
