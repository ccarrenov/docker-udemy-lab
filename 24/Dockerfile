FROM debian 
LABEL version="1.0.0"
LABEL description="Apache + startboostrap freelancer image"
LABEL vendor="ccarrenov"
RUN apt update && apt install apache2 -y
WORKDIR /var/www/html
COPY startbootstrap-freelancer-master/dist .
ENV contenido prueba
RUN echo $contenido > prueba.html
RUN echo $(whoami) > /tmp/user1.html
RUN useradd example
USER example
RUN echo $(whoami) > /tmp/user2.html
USER root
RUN mv /tmp/user1.html /var/www/html
RUN mv /tmp/user2.html /var/www/html 
COPY run.sh /run.sh
CMD sh run.sh
