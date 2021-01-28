FROM php:7.4.14-fpm-alpine
COPY . /app
RUN mv "$PHP_INI_DIR/php.ini-production" "$PHP_INI_DIR/php.ini"
EXPOSE 9000
