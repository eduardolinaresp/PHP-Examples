FROM php:7.2-apache

USER root

RUN apt-get update -y \
  && apt-get install -y \
     libxml2-dev \
	 libfreetype6-dev \
     libjpeg62-turbo-dev \
     libpng-dev \
	 libzip-dev \
     zip \
  && apt-get clean -y \
  && docker-php-ext-install soap \
  && docker-php-ext-install mysqli \ 
  && docker-php-ext-enable mysqli \
  && docker-php-ext-install gd \
  && docker-php-ext-configure zip --with-libzip \
  && docker-php-ext-install zip