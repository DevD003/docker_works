#Dockerfile based on the latest centOS 7 Image - non-priveleged user entry
FROM centos:latest
MAINTAINER DevD003

RUN useradd -ms /bin/bash user

RUN echo "EXPORT 192.168.0.0/24" >> /etc/exports.list

RUN yum update -y  
Run yum install -y net-tools wget

Run cd ~ && wget --no-cookies --no-check-certificate --header "Cookie: gpw_e24=http%3A%2F%2Fwww.oracle.com%2F; oraclelicense=accept-securebackup-cookie" "http://download.oracle.com/otn-pub/java/jdk/8u171-b11/jre-8u171-linux-x64.rpm"

Run yum localinstall -y ~/jre-8u171-linux-x64.rpm

USER user

Run cd ~ && echo "export JAVA_HOME=/usr/java/jdk1.8.171/jre" >> /home/user/.bashrc
