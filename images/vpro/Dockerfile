FROM ubuntu:latest

LABEL "Author"="kemechial"

LABEL "Project"="vpro"

RUN apt update && apt install git -y

RUN  apt install apache2 -y

CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]

EXPOSE 80

WORKDIR /var/www/html

VOLUME /var/log/apache2

ADD vpro.tar.gz /var/www/html 

#copy will just copy, add will untar
 
#COPY  vpro.tar.gz /var/www/html


