FROM docker.io/library/composer:2@sha256:b6dcd72ca98fa19d0e5b8476de179859704891fad06dd9e0b96833d4c430a5fc

RUN pecl bundle -d /usr/src/php/ext apcu \
 && docker-php-ext-install apcu