FROM alpine:3.12
LABEL maintainer="Angga Lanuma <lanuma.angga@gmail.com>"

# RUN apk --no-cache --update add build-base

RUN apk add --no-cache build-base git openssh \
                       nodejs npm bash curl \
                       rsync docker

RUN rc-update add docker boot

RUN curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl"

RUN chmod +x ./kubectl && mv ./kubectl /usr/local/bin/kubectl && kubectl version --client

WORKDIR /app


