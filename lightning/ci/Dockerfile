FROM ubuntu:16.04
MAINTAINER Christian Decker <decker.christian@gmail.com>

RUN echo deb http://ppa.launchpad.net/bitcoin/bitcoin/ubuntu xenial main > /etc/apt/sources.list.d/bitcoin-bitcoin-xenial.list
RUN apt-get update -qq
RUN apt-get install -qq -y --no-install-recommends --allow-unauthenticated \
    asciidoc \
    curl \
    git \
    make \
    automake \
    autoconf \
    libtool \
    bitcoind \
    build-essential \
    libprotobuf-c-dev \
    libsodium-dev \
    libbase58-dev \
    libsqlite3-dev \
    libgmp-dev \
    libsqlite3-dev \
    git \
    net-tools \
    valgrind \
    ca-certificates \
    python \
    python3 \
    python3-pip \
    python3-setuptools \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install python-bitcoinlib==0.7.
RUN mkdir /build
WORKDIR /build
