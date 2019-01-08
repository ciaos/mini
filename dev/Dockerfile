FROM ubuntu:18.04
LABEL maintainer <290979182@qq.com>
ENV VERSION 1.0

RUN cd /root \
    && apt-get update && apt-get install -y apt-utils net-tools sysstat locales git curl wget tar unzip screen subversion iputils-ping vim fish --fix-missing \
    && echo "${TIME_ZONE}" > /etc/timezone && ln -sf /usr/share/zoneinfo/${TIME_ZONE} /etc/localtime

RUN apt-get install -y mysql-client redis mongodb-clients

RUN apt-get install -y software-properties-common && add-apt-repository -y ppa:ondrej/php && apt update \
    && apt install -y php7.1-fpm php7.1-mcrypt php7.1-cli php7.1-xml php7.1-mysql php7.1-gd php7.1-imagick php7.1-recode php7.1-tidy php7.1-xmlrpc php7.1-mbstring php7.1-curl

#RUN apt-get install -y gcc nodejs php php-mysql

#RUN apt-get install -y golang
