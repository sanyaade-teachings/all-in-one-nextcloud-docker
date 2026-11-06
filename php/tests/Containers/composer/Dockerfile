FROM docker.io/library/composer:2@sha256:8de2184c6de224f4689e8f80ed5f5edaf0030b6b8b7839a22a2bcb6722ac87d0

RUN pecl bundle -d /usr/src/php/ext apcu \
 && docker-php-ext-install apcu