
---

## 📘 Lab 7 — Variables & Templates

```markdown
# Lab 7: Variables & Templates

## Objective
Use variables and Jinja2 templates in playbooks.

## Prerequisites
- Ansible installed

## Steps
1. Define variables in `vars.yml`.
2. Create Jinja2 template.
3. Apply template in playbook.

## Commands
```yaml
# vars.yml
app_port: 8080

# template.j2
server {
  listen {{ app_port }};
}

- hosts: servers
  vars_files:
    - vars.yml
  tasks:
    - template:
        src: template.j2
        dest: /etc/nginx/sites-enabled/app.conf
