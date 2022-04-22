####
#   from : https://hub.docker.com/layers/php/library/php/7.4.29-fpm/images/ sha256-26ec7f68fdbd644692cd99b22f566b39ec7026f2bb0feec8d442dfc273af9114?context=explore
####

FROM php:7.4.29-fpm

####
# If you have your own library, you can customize it
####

# RUN apt-get update && apt-get install -y \
# libfreetype6-dev \
# libjpeg62-turbo-dev \
# libmcrypt-dev \
# libpng12-dev \
RUN docker-php-source extract \
  && docker-php-ext-install mysqli \
  && docker-php-ext-install pdo_mysql \