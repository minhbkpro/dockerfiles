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
    composer

# install node, npm, webpack
RUN curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
RUN apt-get install -y nodejs
RUN npm install -g webpack webpack-cli --no-optional

# install codeception
RUN curl -LsS https://codeception.com/codecept.phar -o /usr/local/bin/codecept
RUN chmod a+x /usr/local/bin/codecept
