FROM mcr.microsoft.com/devcontainers/base:dev-ubuntu-22.04

# Avoid warnings by switching to noninteractive
ENV DEBIAN_FRONTEND=noninteractive

# Configure apt and install packages
RUN apt-get update \
    && apt-get -y install --no-install-recommends \
    autoconf \
    bison \
    build-essential \
    curl \
    git \
    iproute2 \
    iputils-ping \
    libgdbm-dev \
    libffi-dev \
    libncurses5-dev \
    libreadline-dev \
    libsqlite3-dev \
    libssl-dev \
    libyaml-dev \
    lldb \
    locales \
    netcat \
    openssh-client \
    procps \
    sqlite3 \
    sudo \
    unzip \
    vim \
    wget \
    zip \
    zlib1g-dev \
    zsh \
    && apt-get autoremove -y \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

# Install Ruby
RUN wget https://cache.ruby-lang.org/pub/ruby/3.2/ruby-3.2.2.tar.gz \
    && tar -xzvf ruby-3.2.2.tar.gz \
    && cd ruby-3.2.2 \
    && ./configure \
    && make \
    && make install \
    && cd .. \
    && rm -rf ruby-3.2.2 \
    && rm ruby-3.2.2.tar.gz

# Install bundler
RUN gem install bundler
