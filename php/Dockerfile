FROM php:7.4.12-fpm

MAINTAINER zhoukan "zkshpro@163.com"

RUN apt-get update \
	&& apt-get install vim -qqy \
    && docker-php-ext-install bcmath pdo_mysql
