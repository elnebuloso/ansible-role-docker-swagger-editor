# Ansible Role - Swagger Editor for Docker

![abandoned](https://img.shields.io/badge/project-abandoned-red)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

- [`defaults/main.yml`](https://github.com/elnebuloso/ansible-role-docker-swagger-editor/blob/master/defaults/main.yml)

## Example Playbook

```
- hosts: localhost
  roles:
    - role: elnebuloso.docker-swagger-editor
      docker_swagger_editor_proxy_name: "swagger-editor.box.entwickl.de"
```

## Dependencies

- `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).
- If Apache2 is installed, a proxy vhost will be configured.

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)