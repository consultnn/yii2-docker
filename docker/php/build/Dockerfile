FROM php:5.6-fpm
# Install modules
RUN apt-get update && apt-get install -y zlibc zlib1g zlib1g-dev --no-install-recommends && rm -r /var/lib/apt/lists/*
RUN docker-php-ext-configure mbstring
RUN docker-php-ext-install mbstring zip

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer && composer global require --prefer-dist "fxp/composer-asset-plugin:~1.0"

CMD ["php-fpm"]