FROM debourge/base:latest
MAINTAINER Derek Bourgeois <debourge@cisco.com>

# add some repositories
RUN apt-add-repository ppa:chris-lea/redis-server -y && \
    apt-get update

# clean up our mess
RUN apt-get remove --purge -y software-properties-common && \
    apt-get autoremove -y && \
    apt-get clean && \
    apt-get autoclean && \
    echo -n > /var/lib/apt/extended_states && \
    rm -rf /var/lib/apt/lists/* && \
    rm -rf /usr/share/man/?? && \
    rm -rf /usr/share/man/??_*
