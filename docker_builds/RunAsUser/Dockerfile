#Dockerfile based on the latest centOS 7 Image - non-priveleged user entry
FROM centos:latest
MAINTAINER DevD003

RUN useradd -ms /bin/bash user

RUN echo "EXPORT 192.168.0.0/24" >> /etc/exports.list

USER user
