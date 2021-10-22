FROM ubuntu:18.04

RUN sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update

RUN apt install -y \
    bash-completion \
    htop \
    vim \
    netcat \
    smem \
    net-tools \
    iputils-ping \
    silversearcher-ag \
    apt-file

RUN apt-file update

