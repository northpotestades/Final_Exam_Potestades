FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y nagios3 nagios-nrpe-plugin apache2

RUN a2enmod cgi && systemctl enable apache2

EXPOSE 80
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
