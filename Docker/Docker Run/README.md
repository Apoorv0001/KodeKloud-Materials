# Basic Run Commands
Run -tag

``` docker run redis:4.0 ```
If we use colon and give version number then the docker pull an image with docker 4.0 version.

## Docker Host
The underlying host where Docker is installed is called Docker host or Docker Engine.

## Run - PORT mapping

```docker run -p 80:5000 kodekloud/webapp```
We can run as many applications and map them to as many ports according to our needs. We cannot port to the docker host more than once on the same port number.

## RUN - Volume mapping

``` docker run mysql ``` 
If we delete the container so it will blow away. So keep it safe we can follow volume mapping and can create another directory called /opt/datadir and map that to /var/lib/mysql .

```docker run -v /opt/datadir:/var/lib/mysql```

## Inspect Container

```docker inspect blissful_hopper```
If we want to see additional details about specific container we can provide container name or container id. It will return all details of a container in a JSOn format. 

## Container Logs
 To see cotainer logs that run in the backgroud. We can specify the container name or container id like this.
 
 ``` docker logs blissful_hopper```