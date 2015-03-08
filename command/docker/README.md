# docker

Linux container management.

"Containers" are working machines started from "images".


## Help

Print a list of commands:

	docker

Print help on a single command:

	docker help run


## Commands

### Manage containers

- [rm](./rm/) to delete a non-running container.

- [run](./run/) to run a command in a new container.

- [start](./start/) to start a stopped container.

- [stop](./stop/) to stop a running container.


### Manage images

- [rmi](./rmi/) to delete an image.

- `pull` to download an image.

- `push` to upload an image.


### View resources

- [images](./images/) to print images.

- [logs](./logs/) to print the output of a container.

- [port](./port/) to print ports used by containers.

- [ps](./ps/) to print running containers.

- [top](./top/) to print processes running in a container.
