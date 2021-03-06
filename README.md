# docker

[![Build Status](https://travis-ci.org/m31271n/ansible-role-docker.svg?branch=master)](https://travis-ci.org/m31271n/ansible-role-docker)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-m31271n.docker-blue.svg)](https://galaxy.ansible.com/m31271n/docker/)

Ansible role that installs docker on EL.

## Supported EL versions

+ 7

## Requirements

None.

## Role Variables

+ `docker_version`: `17.03.1.ce`
+ `docker_users`: `[]`
+ `docker_storage_driver`: `overlay`
+ `docker_http_proxy`: ` `
+ `docker_https_proxy`: ` `
+ `docker_no_proxy`: ` `

Read [here](https://docs.docker.com/engine/admin/systemd/) for HTTP/HTTPS proxy settings.

## Dependencies

None.

## Example Playbook

```
- hosts: servers
  roles:
    - role: m31271n.docker
      docker_version: 17.03.1.ce
      docker_users: [ 'deploy' ]
```

* * *

<p align="center">Made with ❤ by <a href="http://index.m31271n.com">m31271n</a></p>
