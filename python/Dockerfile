FROM undeadops/alpine-base:3.3

MAINTAINER Mitch Anderson <@undeadops>

RUN apk add --update \
    python \
    python-dev \
    py-pip \
    build-base \
    wget \
    supervisor \
  && rm -rf /var/cache/apk/*

RUN mkdir /source
