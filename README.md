# ansible-role-nginx

## Purpose
This ansible role installs Nginx in Docker

## Install
```bash
ansible-galaxy role install m-shalenko.nginx
```

## Example of playbook
```yaml
---
- name: Install Nginx
  hosts: nginx
  become: true
  gather_facts: false
  roles:
    - role: m-shalenko.nginx
      tags:
        - nginx
```
