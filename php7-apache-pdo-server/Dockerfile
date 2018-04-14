FROM php:7.2-apache
RUN docker-php-ext-install pdo pdo_mysql mysqli
COPY ./my-virtual-host.conf /etc/apache2/sites-available/
RUN a2ensite my-virtual-host.conf
RUN a2dissite 000-default.conf
#RUN service apache2 restart

#docker build -t attend_server:1.0 .
