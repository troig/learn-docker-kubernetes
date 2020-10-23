[![Build Status](https://travis-ci.org/troig/learn-docker-kubernetes.svg?branch=develop)](https://travis-ci.org/troig/learn-docker-kubernetes)

## Available Scripts

In the project directory, you can run:

### Build with docker (dev)
docker build -f .\Dockerfile.dev .

### Build with docker (prod)
docker build .

### Run with docker
docker run -it -p 3000:3000 -e CHOKIDAR_USEPOLLING=true -v /app/node_modules -v ${pwd}:/app CONTAINER_ID

### Run with docker compose
docker-compose up

### Run tests with docker
docker run --it CONTAINER_ID npm run test

### Run with nginx
docker run -p 8080:80 CONTAINER_ID
