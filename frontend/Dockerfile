FROM php:7.4-apache-buster

RUN apt update

RUN apt -y install zip unzip git-all

COPY . .

COPY --from=composer:2 /usr/bin/composer /usr/bin/composer

RUN composer update