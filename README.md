# Dockerized Express APP

Bootstrap Dockerized + Docker Compose Node Express APP.

```sh
# create image
docker build -t apps/dockerized-node-micro .
# list images
docker images
# Run image
docker run -p 49160:8080 -d apps/dockerized-node-micro
# Get container ID
docker ps
# Get logs
docker logs <container id>
# log into container
docker exec -it <container id> /bin/bash
```

## Using Docker Compose
* Run `docker-compose up` (needs [Docker Compose](https://docs.docker.com/compose/) installed).


## Test
Make `curl -i localhost:49160` or visit [http://localhost:49160](http://localhost:49160).

## Environment
Add to `.env` if any environment needed inside the container.

## Requirements
* [Docker Engine](https://docs.docker.com/installation/).
* [Docker Compose](https://docs.docker.com/compose/).
* [Docker Machine](https://docs.docker.com/machine/) (Mac and Windows only).

## Credit
* [NodeJs Docker Docs](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/).

