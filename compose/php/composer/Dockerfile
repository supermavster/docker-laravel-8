FROM composer:latest

# ADD and set Group
RUN addgroup -g 1000 laravel && adduser -G laravel -g laravel -s /bin/sh -D laravel

# Set Profile to All Files
RUN chown -R laravel:laravel /var/www/html

# Run in work space
WORKDIR /var/www/html