FROM debian:stable
MAINTAINER djinn3 <adithyakesineni@gmail.com>

RUN apt-get update && apt-get upgrade &&  apt-get install -y apache2 telnet elinks openssh-server 

ENV MYVALUE my-value
ENV CREATOR ADIE

EXPOSE 80
EXPOSE 22

CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]  
