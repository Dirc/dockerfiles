# Image based on centos 7 and start apache service

FROM centos:latest
MAINTAINER e.e.cornet@gmail.com

RUN yum install -y wget
RUN wget https://dl.fedoraproject.org/pub/epel/6/x86_64/epel-release-6-8.noarch.rpm
RUN rpm -Uvh epel-release-6-8.noarch.rpm
RUN yum update -y
RUN yum install -y \
        which \
	sudo \
	httpd \
	php \
	openssh-server \
	openssh-clients

RUN echo "This is a custom index file" > /var/www/html/index.html

EXPOSE 22 80

RUN echo "/usr/sbin/apachectl -DFOREGROUND" >> /root/.bashrc

