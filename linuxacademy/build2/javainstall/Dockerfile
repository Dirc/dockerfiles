# based on latest CentOS 7 - non-priv user entry

FROM centos:latest
MAINTAINER e.e.cornet@gmail.com

RUN echo "EXPORT 192.168.0.0/24" >> /tmp/export.list

RUN useradd -ms /bin/bash user
USER user

