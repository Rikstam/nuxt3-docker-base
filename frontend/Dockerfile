FROM node:16-buster-slim as development

WORKDIR /usr/src/frontend

ENV NPM_CONFIG_PREFIX=/home/node/.npm-global
ENV PATH=$PATH:/home/node/.npm-global/bin
EXPOSE 3000
ENV HOST=0.0.0.0

COPY ./package.json .
COPY ./package-lock.json .

RUN npm install

COPY . .
