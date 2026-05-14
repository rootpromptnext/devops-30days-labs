
---

## 📘 Lab 5 — Jupyter Notebook in Podman

```markdown
# Lab 5: Jupyter Notebook in Podman

## Objective
Run Jupyter Notebook inside a container.

## Prerequisites
- Podman installed
- Python image available

## Steps
1. Pull Jupyter image.
2. Run container with port mapping.
3. Access notebook in browser.

## Commands
```bash
podman run -p 8888:8888 jupyter/base-notebook
