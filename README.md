# my_docker

This is my Docker for basic DEVELOPMENT!

Requirement:
- [Docker](https://docs.docker.com/get-docker/)

## Services
 - web server (nginx) [localhost](http://localhost/)
 - app (PHP 8.1 & composer)
 - database (mysql 8.0)
 - cache (redis) -  OPTIONAL - commented
 - debug (xdebug) - requires [this chrome extension](https://chrome.google.com/webstore/detail/xdebug-helper/eadndfjplgieldjbigjakmdgkmoaaaoc)

## Commands
```bash
docker compose up     # compose/create the container(s)
docker compose up -d  # compose/create the container(s) in detatch mode
docker compose up --build -d  # build images


docker ps           # List containers
docker compose ps   # List services

docker exec -it [CONTAINER] [COMMAND]
docker exec -it my_docker-web-1 bash
docker exec -it my_docker-web-1 sh

# set env variable
# linux
#XDEBUG_MODE=off docker compose up
# windows 
set XDEBUG_MODE=off&& docker compose up &set XDEBUG_MODE=
```


