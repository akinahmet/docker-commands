## Basic Docker Commands

### Docker Container Commands

Create a new container without starting it.

```text
docker create 
```

Rename an existing container

```text
docker rename [CONTAINER_NAME] [NEW_CONTAINER_NAME]
```

Create docker container from a docker image.

```text
docker run 
```

```text
docker run --rm [IMAGE] # removes a container after it exits.

docker run -td [IMAGE] # starts a container and keeps it running.

docker run -it [IMAGE] # starts a container, allocates a pseudo-TTY connected to the container’s stdin, and creates an interactive bash shell in the container.

docker run -it-rm [IMAGE] # creates, starts, and runs a command inside the container. Once it executes the command, the container is removed.
```

Delete a container (if it is not running).

```text
docker rm 
```

Attach Terminal to running container

```text
docker attach
```


Update the configuration of one or more containers.


```text
docker update 
```
Start a container

```text
docker start 
```
Stop a running container

```text
docker stop 
```

Stop a running container and start it up again.

```text
docker restart 
```

### Docker Image Commands

Create an image from a Dockerfile

```text
docker build [URL]
```

Pull an image from a registry

```text
docker pull [IMAGE]
```

Push an image to a registry

```text
docker push [IMAGE]
```

### Docker Commands for Information

Shows running containers.

```text
docker ps
```

All info about a container

```text
docker inspect
```

List real-time events from a container.


```text
docker events [CONTAINER]
```


### Docker Network Commands

List networks

```text
docker network ls
```

Remove network(s)

```text
docker network rm [NETWORK]
```

Show information.

```text
docker network inspect [NETWORK]
```

Connects a container to a network

```text
docker network connect [NETWORK] [CONTAINER]
```

Disconnect a container from a network

```text
docker network disconnect [NETWORK] [CONTAINER]
```

### Docker Management Commands:

```text
  builder     Manage builds
  config      Manage Docker configs
  container   Manage containers
  context     Manage contexts
  image       Manage images
  manifest    Manage Docker image manifests and manifest lists
  network     Manage networks
  node        Manage Swarm nodes
  plugin      Manage plugins
  secret      Manage Docker secrets
  service     Manage services
  stack       Manage Docker stacks
  swarm       Manage Swarm
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes
  ```