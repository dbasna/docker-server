FROM debian:jessie

# Install common / shared packages
RUN apt-get update && apt-get install -y \
    vim

# Install apache & fastcgi
RUN apt-get update && apt-get install -y \
    apache2 \
    libapache2-mod-fcgid

# Modules apache2
RUN a2enmod rewrite proxy_fcgi && \
    service apache2 restart;

# Running apache2 in foreground
RUN rm /etc/apache2/sites-enabled/000-default.conf
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
