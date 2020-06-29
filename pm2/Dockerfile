FROM node:12.18.1-alpine3.9
LABEL maintainer="Angga Lanuma <lanuma.angga@gmail.com>"

RUN apk add --no-cache git openssh nodejs npm bash curl rsync \
    && npm install pm2@latest -g

WORKDIR /app


