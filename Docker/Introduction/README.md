## Introduction:
Docker is a very popular and powerful open-source containerization platform that is used for building, deploying, and running applications. Docker allows us to decouple the application/software from the underlying infrastructure.
<!--  -->
## Why do we need Docker:- 
Compatibility issue
Long setup time
Different dev/Test/Prod environments

## What is Container?
Containers are completely isolated environments as they have their own processes, services, network interfaces they all share the same os kernel.

Different types of Containers are:
LXC, LXD, LXCFS

Docker utilizes LXC Containers.
Public docker repository is called docker hub or docker store.

## What is Image?
An Image is a package or template just like VM Template. It is used to create one or more containers.
While containers are running instances of images that are isolated and have their own environments and set of processes.

## Basic Docker Commands:

Docker run command is use to run a container from an image. 

pull -download the image

``` docker run nginx ```
Running the docker run nginx command will run an instance of the nginx application on the Docker host. If image is not already exists they it will go to the docker hub and pull the image down.

ps -list containers

``` docker ps ```
Docker ps command lists all running containers and some basic information about them such as container Id and name of the image we used to run the containers.

``` docker ps -a ```
-a option  is used to see all containers are running or not.

STOP -stop a container

``` docker stop silly_samet ```
To stop the container use the docker stop command. but we need to provide either the container id or container name.

Rm - Remove a container

``` docker rm silly_sammet ```
Docker rm command is used to terminate or stop container permanently. and for confirming run docker ps command.

images- List images
``` docker images ```
The docker iimages command to see a list of available images and their sizes.

rmi- remove images
``` dokcer rmi nginx ```
To remove images make sure that no containers are runnning off of that image before attempting to remove.

Pull - download an image
``` docker pull nginx ```
Docker pull command is used to pull image and not run the container 
