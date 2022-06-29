#UNZIP
unzip startbootstrap-freelancer.zip
#CREATE IMAGE
docker build -t apache .
#CREATE CONTAINER FROM IMAGE
docker run -d --name apache_container -p 80:80 apache
#LIST RUN CONTAINER
docker ps 
#STOP CONTAINER 
docker stop apache_container
#REMOVE CONTAINER
docker rm apache_container
