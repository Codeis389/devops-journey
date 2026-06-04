# Day 2 - Dcoker

## Table of Content
- Docker installed
- Dockerfile created
- Docker image built
- Site running in Docker container

## What is Docker
- Packages app in a container
- Runds identically anywhere
- Like a shipping container for software

## Commands I Learned
docker build -t name .     -----------  build image
docker run -d -p 8080:80   -----------  run container
docker ps                  -----------  see running containers
docker pas -a              -----------  see all container
docker stop ID             -----------  stop container
docker images              -----------  see all images

## Dockerfile I Created
FROM nginx:alpine
COPY ./user/share/nginx/html
EXPOSE 80

## My Site Running in Docker
http://localhost:8080


## Some Useful Docker Commands To Know

- sudo docker ps  =  See running containers
- sudo docker ps -a  = See all containers including stopped
- sudo docker stop CONTAINER_ID  =  Stop a container
- sudo docker start CONTAINER_ID =  Start a container again
- sudo docker rm CONTAINER_ID  =  Delete a container
- sudo docker images  =  See all images
- sudo docker rmi IMAGE_NAME
