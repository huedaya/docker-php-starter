FROM php:8.0-apache

# Install Composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Install unzip utility and libs needed by zip PHP extension
RUN apt-get update && apt-get install -y \
    zlib1g-dev \
    libzip-dev \
    unzip
RUN docker-php-ext-install zip

# Install git
RUN apt-get update && apt-get -y install git

# Install Mysql
RUN docker-php-ext-install pdo pdo_mysql mysqli
RUN a2enmod rewrite
