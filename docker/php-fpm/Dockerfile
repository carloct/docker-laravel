FROM php:fpm

RUN apt-get update && apt-get install -y \
  libmcrypt-dev && \
  docker-php-ext-install pdo_mysql mcrypt