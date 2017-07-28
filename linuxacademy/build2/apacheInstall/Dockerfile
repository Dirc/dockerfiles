# Image based on centos 7 and start apache service

FROM centos:latest
MAINTAINER e.e.cornet@gmail.com

RUN yum update -y
RUN yum install -y httpd net-tools

RUN echo "This is a custom index file" > /var/www/html/index.html

EXPOSE 80

ENTRYPOINT apachectl "-DFOREGROUND"

