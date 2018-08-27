#Image Based on CentOS 7 and Start Apache Service in each container

FROM centos:latest
MAINTAINER DevD003

RUN yum update -y 
RUN yum install -y httpd net-tools

RUN echo "This is a custom index file build during the image creation" > /var/www/html/index.html

EXPOSE 80

ENTRYPOINT apachectl "-DFOREGROUND" 

 
