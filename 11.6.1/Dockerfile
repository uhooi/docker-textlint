FROM node:12.14.1-alpine3.11
LABEL maintainer="uhooi <the_uhooi@yahoo.co.jp>"

ARG VERSION="11.6.1"

RUN set -x && \
    npm install -g textlint@${VERSION} \
    textlint-rule-preset-ja-technical-writing@3.1.3 \
    textlint-filter-rule-comments@1.2.2 \
    textlint-plugin-review@0.4.0 \
    power-assert@1.6.1 && \
    npm cache clean --force

WORKDIR /work
ENTRYPOINT ["/usr/local/bin/textlint"]

