FROM ubuntu:16.04
MAINTAINER liuke (1451790757@qq.com)
RUN apt-get update && apt-get install -y openssh-server git make gawk gcc unzip bzip2 g++ \
	libncurses5-dev zlib1g-dev autoconf gettext asciidoc subversion bsdmainutils iputils-ping \
	libnet-ifconfig-wrapper-perl lrzsz

RUN mkdir /var/run/sshd
ENV LANG=C.UTF-8
WORKDIR /share
EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
