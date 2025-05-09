# Docker Role

This role installs and configures Docker and Docker Compose.

## Requirements

- Ansible 2.17+
- Ubuntu 24.04

## Role Variables

- `docker_version`: The version of Docker to install (default: `5:27.5.1-1~ubuntu.24.04~noble`).
- `docker_compose_version`: The version of Docker Compose to install (default: `v2.32.4`).

## Example Playbook

```yaml
- name: Install and Configure Docker
  hosts: all
  become: true
  roles:
    - docker
```
