FROM debian
RUN apt update && apt install apache2 -y
COPY startbootstrap-freelancer-master/dist /var/www/html
CMD apachectl -DFOREGROUND
