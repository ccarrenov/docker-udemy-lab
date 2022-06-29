FROM debian 
COPY startbootstrap-freelancer-master/dist /var/www/html
RUN apt update && apt install apache2 -y
CMD apachectl -DFOREGROUND
