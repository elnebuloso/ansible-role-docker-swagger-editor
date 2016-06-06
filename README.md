# Ansible Role - Swagger Editor for Docker

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-swagger-editor.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-swagger-editor)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
docker_swagger_editor_state: "started"
docker_swagger_editor_version: "v2.9.9"
docker_swagger_editor_container_name: "swagger-editor"
docker_swagger_editor_container_port: "49160"
docker_swagger_editor_proxy_name: "swagger-editor.box.entwickl.de"
docker_swagger_editor_proxy_port: "80"
```

## Example Playbook

```
- hosts: localhost
  vars:
    docker_swagger_editor_proxy_name: "swagger-editor.box.entwickl.de"
  roles:
    - { role: elnebuloso.docker-swagger-editor }
```

## Dependencies

- `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).
- If Apache2 is installed, a proxy vhost will be configured.

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)