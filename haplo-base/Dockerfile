FROM ubuntu:16.04
MAINTAINER Peter Tribble <peter.tribble@haplo-services.com>
ENV PG_VERSION 9.5
RUN apt-get update && apt-get install -y --no-install-recommends \
  avahi-daemon \
  curl \
  g++ \
  git \
  libxapian22v5 \
  make \
  maven \
  openjdk-8-jdk \
  patch \
  software-properties-common \
  sudo \
  supervisor \
  uuid-dev \
  && rm -rf /var/lib/apt/lists/*
RUN apt-get update && apt-get install -y --no-install-recommends \
  postgresql-$PG_VERSION \
  postgresql-server-dev-$PG_VERSION \
  postgresql-contrib-$PG_VERSION \
  && rm -fr /var/lib/postgresql/$PG_VERSION \
  && rm -rf /var/lib/apt/lists/*
