ARG VARIANT="jammy"
FROM buildpack-deps:${VARIANT}-curl

LABEL dev.containers.features="common"

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && yes | unminimize 2>&1 
