FROM php:7.0-apache
RUN a2enmod rewrite
RUN apt-get update
RUN apt-get install -y mysql-client
RUN "zcat /var/www/html/mysql -h db -u omekausername -pomekapassword"

