FROM ubuntu

WORKDIR /usr/src/www

RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    apt-utils \
    zlib1g-dev \
    libicu-dev \
    g++ \
    curl \
    wget \
    git \
    php \
    php-mysql \
    php-intl \
    php-mbstring \
    php-simplexml \
    php-zip \
    php-curl \
    composer \
    nodejs \
    npm

# install codeception
RUN curl -LsS https://codeception.com/codecept.phar -o /usr/local/bin/codecept
RUN chmod a+x /usr/local/bin/codecept
