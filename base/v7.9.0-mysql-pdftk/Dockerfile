FROM node:7.9.0

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update
RUN apt-get install -y mysql-client libmysqlclient-dev
RUN apt-get install -y pdftk

RUN apt-get clean \
  && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/
