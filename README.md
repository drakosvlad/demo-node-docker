# Demo Node app in Docker

Vladyslav Bozhko

[Link to Docker hub](https://hub.docker.com/repository/docker/multipod/demo-node-docker/general)

## Running with docker-compose

1. Build the image: `docker-compose build`
2. Start the container: `docker-compose up -d`
3. Push the image: `docker-compose push`

## Running without docker-compose

1. Build the image: `docker build . -t multipod/demo-node-docker:latest`
2. Start the container: `docker run -p 80:8080 -m 128m --cpus=0.5 -d demo-node-docker`
3. Push the image: `docker push multipod/demo-node-docker:latest`

## Run the server directly

```
yarn
node src/index.mjs
```