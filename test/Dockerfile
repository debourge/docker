FROM debourge/base:latest
MAINTAINER Derek Bourgeois <debourge@cisco.com>

# add some repositories
RUN apt-add-repository ppa:nginx/stable -y && \
    apt-add-repository ppa:chris-lea/redis-server -y && \
    apt-get update
