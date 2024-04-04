FROM php:8.2-cli
LABEL maintainer="Jaivic"

RUN apt-get update && apt-get -y install zlib1g-dev libicu-dev libxml2-dev libpq-dev vim \
        && docker-php-ext-configure pgsql -with-pgsql=/usr/local/pgsql
        #&& docker-php-ext-install pdo pdo_mysql pdo_pgsql zip intl xmlrpc soap opcache \
        #&& docker-php-ext-configure pdo_mysql --with-pdo-mysql=mysqlnd 

COPY  . /var/www/html/
WORKDIR /var/www/html/

