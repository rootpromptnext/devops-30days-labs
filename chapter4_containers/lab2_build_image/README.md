
---

## 📘 Lab 2 — Build Image

```markdown
# Lab 2: Build Custom Image

## Objective
Build a custom container image using Podman.

## Prerequisites
- Podman installed
- Dockerfile prepared

## Steps
1. Create Dockerfile with sample app.
2. Build image.
3. Run container.

## Commands
```bash
podman build -t myapp:1.0 .
podman run -p 8080:8080 myapp:1.0
