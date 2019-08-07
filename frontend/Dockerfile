#Docker file for Apache Sample Application

FROM centos:7
MAINTAINER sandilyasd@gmail.com
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
EXPOSE 80
COPY config/httpd-foreground /usr/bin
RUN chmod 755 usr/bin/httpd-foreground
CMD ["httpd-foreground"]