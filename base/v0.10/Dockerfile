FROM google/debian:wheezy

RUN apt-get update -y && apt-get install --no-install-recommends -y -q curl python build-essential git ca-certificates
RUN mkdir /nodejs && curl http://nodejs.org/dist/v0.10.41/node-v0.10.41-linux-x64.tar.gz | tar xvzf - -C /nodejs --strip-components=1

ENV PATH bin:node_modules/.bin:/nodejs/bin:$PATH
