FROM php:7.2-fpm

RUN apt-get update && apt-get install -y \
  libmcrypt-dev && \
  docker-php-ext-install pdo_mysql mcrypt

RUN pecl channel-update pecl.php.net \
  && pecl install xdebug-2.6.1 \
  && docker-php-ext-enable xdebug

COPY xdebug.ini /usr/local/etc/php/conf.d/xdebug.ini