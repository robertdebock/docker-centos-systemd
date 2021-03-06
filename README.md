Docker CentOS Systemd
=====================

This Dockerfile can build containers capable to use systemd.

[![centos build status](https://img.shields.io/docker/cloud/build/robertdebock/centos.svg)](https://hub.docker.com/repository/docker/robertdebock/centos)

Branches
--------

This repository has multiple branches that relate to CentOS versions.

|Branch |CentOS Version|Docker image tag|
|-------|--------------|----------------|
|master |latest (8)    |8               |
|7      |7             |7               |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
docker run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  robertdebock/centos
```
