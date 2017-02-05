FROM php:5.6
RUN apt-get update \
  && apt-get install -y libfreetype6-dev libjpeg62-turbo-dev libpng12-dev libmcrypt-dev git \
  && docker-php-ext-install pdo_mysql mysqli mbstring gd iconv mcrypt \
  && curl -sS https://getcomposer.org/installer | php \
  && mv composer.phar /usr/local/bin/composer 

WORKDIR /app
CMD php -S 0.0.0.0:8080 -t public
