FROM docker.io/library/composer:2@sha256:50ea4d33fdcde1adb0f045547295faa1548b33872e5f789dae5b02ce2fb5de93

ARG APCU_VERSION=5.1.28

SHELL ["/bin/ash", "-o", "pipefail", "-c"]
RUN mkdir -p /usr/src/php/ext/apcu \
 && curl -fsSL --retry 5 "https://github.com/krakjoe/apcu/archive/refs/tags/v$APCU_VERSION.tar.gz" \
  | tar -xz --strip-components=1 -C /usr/src/php/ext/apcu \
 && docker-php-ext-install apcu
