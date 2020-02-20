####################################
# NODE                             #
####################################
FROM ubuntu:bionic

LABEL maintainer="Radek Hrebecek <radek@hrebecek.cz>"

# Fixes some weird terminal issues such as broken clear / CTRL+L
ENV TERM=linux

# Ensure apt doesn't ask questions when installing stuff
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
    && apt-get install -y --no-install-recommends gnupg ca-certificates unzip curl \
    && curl -sL https://deb.nodesource.com/setup_12.x | bash - \
    && apt-get update \
    && apt-get -y --no-install-recommends install nodejs \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*

# Work dir per project
WORKDIR /var/www

ENTRYPOINT ["npm"]