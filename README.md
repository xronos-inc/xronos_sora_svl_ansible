# Run SORA-SVL

Run SORA-SVL in a docker network.

See [xronos-inc/sora-svl](http://github.com/xronos-inc/sora-svl) for source of the Docker images. Special thanks to the original author of SORA-SVL, [YuqiHuai](https://github.com/YuqiHuai).

The docker images are hosted by DensoSVIC:

- [densosvic/sora-svl-server](https://hub.docker.com/repository/docker/densosvic/sora-svl-server)
- [densosvic/sora-svl-client](https://hub.docker.com/repository/docker/densosvic/sora-svl-client/)
- [densosvic/sora-svl-mongo](https://hub.docker.com/repository/docker/densosvic/sora-svl-mongo/)
- [densosvic/sora-svl-router](https://hub.docker.com/repository/docker/densosvic/sora-svl-router/)
- [densosvic/sora-svl-docs](https://hub.docker.com/repository/docker/densosvic/sora-svl-docs/)

## Features

- Pulls SORA-SVL docker images
- Creates a docker network and runs containers

## OS support

- Ubuntu 22.04
- Ubuntu 24.04

Platforms supported:

- linux/amd64
- linux/arm64

## Prerequisites

- Ansible 2.15

## Example playbook

```yaml
roles:
  - name: xronos_sora_svl_ansible
    role: xronos_sora_svl_ansible
```

## Variables

- `sora_svl_version` SORA-SVL version to pull from Docker. Defaults to empty (latest).
