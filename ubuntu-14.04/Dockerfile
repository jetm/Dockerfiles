FROM ubuntu:14.04
MAINTAINER Javier Tia <javier.tia@gmail.com>
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install -y \
    build-essential  \
    devscripts \
    fakeroot \
    quilt \
    dh-make \
    automake \
    libdistro-info-perl \
    less \
    cmake \
    git \
    libpcap-dev \
    bzr-builder
RUN apt-get clean

RUN adduser --ingroup users --disabled-password \
    --gecos 'User to develop' john

