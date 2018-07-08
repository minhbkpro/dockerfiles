FROM php:7.2-fpm

WORKDIR /usr/src/www

RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    zlib1g-dev \
    libicu-dev \
    g++

RUN docker-php-ext-install \
    mysqli \
    pdo \
    pdo_mysql \
    intl
