FROM docker.io/library/composer:2@sha256:4ed71c38c6d788eb4e4e3747b5332f5b40d5b5a6fcadd5062a1a70986a118e0a

RUN pecl bundle -d /usr/src/php/ext apcu \
 && docker-php-ext-install apcu