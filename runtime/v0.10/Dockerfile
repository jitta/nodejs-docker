FROM jitta/nodejs:v0.10

# ENV
# some app try to detect root user in this case 'foreman'
ENV NODE_ENV production
ENV SUDO_USER root
EXPOSE 3000

# Dependency 
WORKDIR /app
ONBUILD ADD package.json /app/package.json
ONBUILD ADD node_modules /app/node_modules
ONBUILD RUN npm install && npm install -g foreman

# Add all project
ONBUILD ADD . /app

CMD []
ENTRYPOINT ["/nodejs/bin/nf", "start"]
