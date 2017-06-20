FROM node:8.1.2

ENV DEBIAN_FRONTEND noninteractive

# Install MySQL Client
RUN apt-key adv --keyserver pgp.mit.edu --recv-keys 5072E1F5
RUN echo "deb http://repo.mysql.com/apt/debian/ jessie mysql-5.7" > /etc/apt/sources.list.d/mysql.list
RUN apt-get update
RUN apt-get install -y mysql-client libmysqlclient-dev
RUN apt-get clean \
  && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/
