FROM ubuntu:16.04
MAINTAINER Derek Bourgeois <debourge@cisco.com>

# configure the container
RUN DEBIAN_FRONTEND=noninteractive

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

# create non-root user
ARG PUID=1000
ARG PGID=1000
RUN groupadd -g $PGID ubuntu && \
    useradd -u $PUID -g ubuntu -m ubuntu
