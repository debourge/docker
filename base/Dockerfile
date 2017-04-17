FROM ubuntu:16.04
MAINTAINER Derek Bourgeois <debourge@cisco.com>

# configure the container
RUN DEBIAN_FRONTEND=noninteractive
RUN locale-gen en_US.UTF-8

ENV LANGUAGE=en_US.UTF-8
ENV LC_ALL=en_US.UTF-8
ENV LC_CTYPE=en_US.UTF-8
ENV LANG=en_US.UTF-8

# update the container
RUN apt-get update && \
    apt-get upgrade -y

# install some basics
RUN apt-get install -y \
    software-properties-common \
    git \
    curl \
    nano
