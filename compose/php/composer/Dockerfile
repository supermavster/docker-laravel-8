FROM composer:latest

# ADD and set Group
RUN addgroup -g 1000 laravel && adduser -G laravel -g laravel -s /bin/sh -D laravel

# Run in work space
WORKDIR /var/www/html