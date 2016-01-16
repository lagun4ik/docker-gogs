Dockerized GOGS stack [![Build Status](https://travis-ci.org/lagun4ik/docker-gogs.svg?branch=master)](https://travis-ci.org/lagun4ik/docker-gogs)
--------------------------

Docker-compose file for [gogs](http://gogs.io) server(a self-hosted git service).

>Gogs:latest, MariaDB:10.1

## Run

```bash
docker-compose -p gogs  up -d
```

## Mysql authorization
```yml
MYSQL_DATABASE: gogs
MYSQL_USER: gogs
MYSQL_PASSWORD: gogs
```

## Show services

```bash
docker-compose -p gogs ps
```

## Look at the logs

```bash
# all logs
docker-compose -p gogs logs

# specific service
docker-compose -p gogs logs mysql
```
