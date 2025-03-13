# Use PHP 5.5.38 with Apache as the base image
FROM php:5.5.38-apache

# Install MySQLi and PDO MySQL extensions
RUN apt-get update && apt-get install -y libmysqlclient-dev \
    && docker-php-ext-install mysqli pdo_mysql

# Enable Apache mod_rewrite
RUN a2enmod rewrite

# Expose the default port
EXPOSE 80
