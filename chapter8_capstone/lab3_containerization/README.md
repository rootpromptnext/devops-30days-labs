# Lab 3: Containerization

## Objective
Containerize the capstone application.

## Prerequisites
- Podman installed
- App code ready

## Steps
1. Write Dockerfile.
2. Build image.
3. Run container.

## Commands
```bash
podman build -t capstone-app:1.0 .
podman run -p 8080:8080 capstone-app:1.0
```
