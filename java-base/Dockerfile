FROM openjdk:8-jre-alpine

RUN apk update && apk add --no-cache ca-certificates bash wget curl openssl

ENV DOCKERIZE_VERSION v0.3.0
RUN set -x \
        && wget https://github.com/jwilder/dockerize/releases/download/$DOCKERIZE_VERSION/dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
        && tar -C /usr/local/bin -xzvf dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz \
        && rm dockerize-linux-amd64-$DOCKERIZE_VERSION.tar.gz
