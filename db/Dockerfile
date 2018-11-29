FROM postgres:alpine

WORKDIR /usr/src/db

RUN apk add --no-cache build-base git

RUN git clone https://github.com/fairingrey/pg_simple_parser /simple_parser; \
    cd /simple_parser; \
    make install