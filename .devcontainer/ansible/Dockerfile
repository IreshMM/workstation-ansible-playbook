FROM ubuntu:22.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update -y && apt-get upgrade -y
RUN apt-get -y install vim iputils-ping bind9-dnsutils git telnet pipx genisoimage wget jq ipcalc python3-pip ruby-rubygems expect tree locales
RUN apt update -y && \
  apt install -y software-properties-common && \
  add-apt-repository --yes --update ppa:ansible/ansible && \
  apt install -y ansible
RUN locale-gen en_US.UTF-8
RUN git config --global --add safe.directory /workspace