## Basic Docker Commands

### Docker Container Commands

Create a container without starting it.

```text
docker create [IMAGE]
```

Rename an existing container

```text
docker rename [CONTAINER_NAME] [NEW_CONTAINER_NAME]
```

Run a command in a new container

```text
docker run [IMAGE] [COMMAND]
```

```text
docker run --rm [IMAGE] # removes a container after it exits.

docker run -td [IMAGE] # starts a container and keeps it running.

docker run -it [IMAGE] # starts a container, allocates a pseudo-TTY connected to the container’s stdin, and creates an interactive bash shell in the container.

docker run -it-rm [IMAGE] # creates, starts, and runs a command inside the container. Once it executes the command, the container is removed.
```

Delete a container (if it is not running).

```text
docker rm [CONTAINER]
```

Update the configuration of one or more containers.

```text
docker update [CONTAINER]
```
Start a container

```text
docker start [CONTAINER]
```
Stop a running container

```text
docker stop [CONTAINER]
```

Stop a running container and start it up again.

```text
docker restart [CONTAINER]
```
