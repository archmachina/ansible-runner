FROM ubuntu:24.04

ARG DEBIAN_FRONTEND=noninteractive

RUN apt update && apt install -y software-properties-common curl \
  apt-transport-https apt-utils lsb-release gnupg ca-certificates

RUN apt-add-repository --yes --update ppa:ansible/ansible

RUN apt update && apt install -y ansible sshpass

WORKDIR /ansible

ENTRYPOINT [ "/bin/bash" ]
