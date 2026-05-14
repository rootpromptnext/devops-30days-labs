# Lab 6: Install Drone CI

## Objective
Set up Drone CI server for automated builds.

## Prerequisites
- Gitea running
- Docker/Podman installed

## Steps
1. Pull Drone CI image.
2. Run Drone server linked to Gitea.
3. Access Drone UI.

## Commands
```bash
podman run -d --name drone \
  -p 8080:80 \
  -e DRONE_GITEA_SERVER=http://gitea:3000 \
  -e DRONE_GITEA_CLIENT_ID=<client_id> \
  -e DRONE_GITEA_CLIENT_SECRET=<client_secret> \
  drone/drone:latest
