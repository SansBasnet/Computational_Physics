# Docker

##### Images versus containers

An image is the binaries, the libraries and source codes that make up the application. An image is the application we want to run. A container is an instance of that image running as a process.

Docker’s default image “registry” is called Docker Hub (hub.docker.com). Registries are like what GitHub is to source code. 

docker container run --publish 80:80 nginx 

What did this command do?

1. Downloaded image ’ngnix’ from Docker Hub
2. Started a new container from that image 
3. Opened port 80 on the host IP

The publish part of the command exposes my local port 80 on my local machine and sends all traffic from it to the executable running inside that container on port 80. [nginx is a web server.]

4. Routes that traffic to the container IP, port 80
