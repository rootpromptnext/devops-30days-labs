# Lab 1: Install Gitea

## Objective
Set up a self‑hosted Git service using Gitea.

## Prerequisites
- Linux VM or server
- Docker or Podman installed

## Steps
1. Pull Gitea image.
2. Run container with mapped ports.
3. Access Gitea web UI.

## Commands
```bash
podman run -d --name gitea \
  -p 3000:3000 -p 222:22 \
  gitea/gitea:latest
