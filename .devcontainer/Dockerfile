ARG VARIANT="jammy"
FROM buildpack-deps:${VARIANT}-curl

LABEL dev.containers.features="common"

ENV LANG="C.UTF-8"

RUN apt-get update \
    && apt-get upgrade -y \
    && export DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y --no-install-recommends \
        make \
        yarn \
    && rm -rf /var/lib/apt/lists/* \
    && apt-get update \
    && apt-get upgrade -y \
    && rm -rf /var/lib/apt/lists/* \
    && yes | unminimize 2>&1