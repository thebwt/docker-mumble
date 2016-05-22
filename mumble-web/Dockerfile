FROM php:5.6-apache

RUN apt-get update && apt-get install -y \
    php-zeroc-ice \
 && rm -rf /var/lib/apt/lists/*

COPY src/ /var/www/html/
RUN chown -R www-data:www-data /var/www/html
