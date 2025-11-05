# Docker Image with oraclelinux10 base image

This repo was created in order to test ansible roles with molecule.

## Build it locally

  docker build -t oraclelinux10img .
  docker run -d -name oraclelinux10con --cgroupns=host --volume=/sys/fs/cgroup:/sys/fs/cgroup:rw oraclelinux10img
  docker exec -it oraclelinux10con bash

## Use it from dockerhub

    https://hub.docker.com/repository/docker/lotusnoir/ansible_molecule_test_images:oraclelinux10
