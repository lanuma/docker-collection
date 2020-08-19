FROM node:12.18.1-alpine3.9
LABEL maintainer="Angga Lanuma <lanuma.angga@gmail.com>"

ENV PYTHONUNBUFFERED=1
RUN apk add --update --no-cache python3 && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip
RUN pip3 install --no-cache --upgrade pip setuptools

RUN apk add --no-cache git openssh nodejs npm bash curl rsync \
    && npm install pm2@latest -g

WORKDIR /app


