# Docker labs student project.

This project consists of 3 docker images glued into a service with docker-compose.



The structure is as follows:

database - mysql:latest image from dockerhub

php - php:7.4-fpm-alpine from dockerhub

apache httpd - httpd:2.4-alpine from dockerhub




There are two networks:

frontend -> for public services such as httpd

backend -> connects services together so the default one isn't used




There are two volumes:

app_data -> contains php code

database_data -> contains mysql logs

## Setup
```
docker pull httpd:2.4-alpine php:7.4-fpm-alpine mysql:latest
docker-compose build
``` 

## Run
```
docker-compose up 
```

## Run detached
```
docker-compose up -d
```



