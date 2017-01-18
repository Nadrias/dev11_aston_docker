FROM php:7.1.0-apache

ENV TERM=xterm

RUN apt-get update
RUN apt-get install unzip -y


RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
RUN php composer-setup.php
RUN php -r "unlink('composer-setup.php');"
RUN mv composer.phar /usr/bin/composer

RUN apt-get update
RUN apt-get install nano -y
