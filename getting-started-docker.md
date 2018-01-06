# Getting started with Docker

*Updated as of Jan 2018*

Docker hub hosts images that allow us to run containers on our machine.

Container:
+ OS level virtualization

Docker:
+ is great for deployment
+ building consistent development environments for team projects
+ dev environment = production environment
+ avoids overhead of starting and maintaining VMs
+ Can still use your favorite editor/IDE as you normally do. No need for running a VM in VirtualBox and SSHing in and developing from the shell just so you can build/run on a Linux box.

**[Free Udemy Course to get started on Docker](https://www.udemy.com/docker-for-developers/learn/v4/)**
 
## Docker or Docker Toolbox on Windows

+ use [Docker Toolbox](https://docs.docker.com/toolbox/toolbox_install_windows/) if running Windows 10 only. (No Windows 10 Pro)

+  use Docker Toolbox if you use VMware. [Hyper-V on Windows may break VMware config](https://forums.docker.com/t/docker-for-windows-w-vmware-installed/19011)

## docker vs docker-machine

use docker-machine if running Docker Toolbox

## Docker Commands


```
docker login                        #login to docker hub
docker-machine                      #command list
docker-machine start default        #start machine named default
docker-machine kill default         #kill machine named default
docker-machine ip                   #get IP
docker-machine ls                   #list machines
docker pull name                    #pull image from docker hub
docker run name                     #run container
docker images                       #list of images
docker rm 77                        #remove based on first 2 digit of container ID
docker rmi f2                       #remove image based on first 2 digit
```

Using hello-world-nginx
```
docker run -p 80:80
```

`-p` flag for port. 80 (external port) : 80 (internal port)

`-d` detached mode; run container in background

## Layers

An image is a set of read-only layers, container has a thin R/W layer

Containers can share image layers.

## Volume

Special type of directory in a container referred as "data volume"

can be shared and reused among containers

update to an image won't affect data volume

**data volumes are persisted even after the container is deleted**

Customizing the host location for a data volume:
```
docker run -p 8080:3000 -v $(pwd):/var/www node
```

`-v` creates a volume

## Dockerfile

+ simple text file with instructions to create an image

## Building custom images

```
docker build -t <username>/<imagename> .
```

`-t` tag flag to set name

`.` to indicate that dockerfile is in current working directory

## Publish an image on Dockerhub

1. Create a repo

2. Push image to repo
```
docker push <username>/<imagename>
```

[nginx-test](https://hub.docker.com/r/davzoku/nginx-test/)

## Linking Containers

##TODO

## Container Networks

##TODO

## [Docker Swarm](https://www.youtube.com/watch?v=KC4Ad1DS8xU)

Docker swarm is a cluster of machines all running docker which provide a scalable and reliable platform to run many containers

### To run swarm mode:
+ Docker 1.12 and above
+ same subnet
+ ports 2377, 4789, 7946 open
+ TCP port 2377 for cluster management communications
+ TCP and UDP port 7946 for communication among nodes
+ UDP port 4789 for overlay network traffic

### To create a swarm:

To init and set machine with IP of 10.0.0.4 as manager:
```
docker swarm init --listen-addr 10.0.0.4:2377
```
To list all nodes in swarm:
```
docker node ls
```

To join swarm:
```
swarm join 10.0.0.4:2377
``` 

To deploy a service to the swarm:
```
docker service create ...
```

To list all running services:
```
docker service ls
```