FROM ubuntu:18.04
LABEL maintainer <290979182@qq.com>
ENV VERSION 1.0

RUN cd /root \
    && apt-get update && apt-get install -y apt-utils net-tools sysstat locales git curl wget tar unzip screen subversion iputils-ping vim fish \
    && echo "${TIME_ZONE}" > /etc/timezone && ln -sf /usr/share/zoneinfo/${TIME_ZONE} /etc/localtime

RUN apt-get install -y gcc nodejs php


