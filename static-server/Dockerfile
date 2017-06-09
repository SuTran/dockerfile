FROM ubuntu:trusty

RUN apt-get update && \
    apt-get install -qy wget

RUN wget --quiet -O - https://deb.nodesource.com/setup_6.x | sudo -E bash -

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -qy curl nodejs
RUN npm -g install static-server

RUN apt-get clean && rm -rf /var/lib/apt/lists/* /var/tmp/*
