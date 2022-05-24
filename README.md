# Simple Node

## Overview

This is a very simple, bare-bones NodeJS project created for you to use with Docker.

## Local Setup

- Install dependencies: `npm install`
- Run server: `node server.js`

## Container Setup

- Build image: `docker build .`
- Run container with image: `docker run {image_id}` where `image_id` can be retrieved by running `docker images` and found under the column `IMAGE ID`

## Container teardown

- Remove container: `docker kill {container_id}` where `container_id` can be retrieved by running `docker ps` and found under the column `CONTAINER ID`

## Troubleshooting Docker Containers 

- Viewing logs: `docker logs`
- Attaching to a  container: `docker exec -it`
- Viewing Docker Process: `docker ps`
- Viewing Details of Docker Objects: `docker inspect`


## Pushing an Image to DockerHub

- Login to DockerHub `docker login --username={YOUR USERNAME}`
- Tag the image `docker tag simple-node {YOUR USERNAME}/{YOUR REPOSITORY NAME}`
- Push the tagged image to DockerHut `docker push {TAGGED IMAGE}`
- Pull the image back into your local machine `docker pull {TAGGED IMAGE}`
