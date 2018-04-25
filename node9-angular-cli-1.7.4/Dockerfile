FROM node:9.11.1

# install angular-cli as node user
RUN chown -R node:node /usr/local/lib/node_modules \
  && chown -R node:node /usr/local/bin

USER node
RUN npm install -g @angular/cli@1.7.4

# set npm as default package manager for root
USER root
RUN ng set --global packageManager=npm

USER node

ENV PATH "/usr/local/bin/npm:/usr/local/bin/node:/usr/local/bin/ng:$PATH"
