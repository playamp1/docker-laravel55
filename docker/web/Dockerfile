FROM php:7.1.17-fpm-alpine

RUN apk --no-cache add curl libmcrypt-dev zlib-dev git
RUN apk update && apk add nodejs
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin --filename=composer
RUN docker-php-ext-install pdo_mysql mysqli mbstring mcrypt zip
