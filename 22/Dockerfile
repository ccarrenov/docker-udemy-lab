FROM debian 
RUN apt update && apt install apache2 -y
WORKDIR /var/www/html
COPY startbootstrap-freelancer-master/dist .
ENV contenido prueba
RUN echo $contenido > prueba.html
CMD apachectl -DFOREGROUND
