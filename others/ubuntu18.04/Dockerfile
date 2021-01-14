FROM ubuntu:18.04

RUN sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list

RUN apt update

RUN apt install -y \
    bash-completion \
    bash-completion \
    htop \
    vim \
    netcat \
    smem \
    net-tools \
    iputils-ping \
    silversearcher-ag
