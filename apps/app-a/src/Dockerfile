FROM php:8.3-fpm-alpine
WORKDIR /var/www/html

RUN apk add --no-cache tzdata \
 && cp /usr/share/zoneinfo/Europe/Budapest /etc/localtime \
 && echo "Europe/Budapest" > /etc/timezone
COPY src/ /var/www/html/
RUN chown -R www-data:www-data /var/www/html
