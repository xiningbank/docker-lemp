FROM php:7.4.12-fpm

MAINTAINER zhoukan "zkshpro@163.com"

RUN apt-get update \
	&& apt-get install vim -qqy \
	&& apt-get install git -qqy \
	&& apt-get install zip -qqy \
	&& apt-get install unzip -qqy \
    && docker-php-ext-install bcmath \
    && docker-php-ext-install pdo_mysql \
    && pecl install redis && docker-php-ext-enable redis

# install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
