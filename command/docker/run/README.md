# docker run

Run a command in a new container.

A container is stopped once the command is finished.
Use `-d` to keep the container running in the background.


## Hello world

	docker run ubuntu:14.04 /bin/echo 'Hello world'

Specifying image name (ubuntu:14.04), command (/bin/echo) and command
arguments ('Hello world').


## Interactive container

	docker run -t -i ubuntu:14.04 /bin/bash

`-t` creates a terminal and `-i` allows us to provide input.


## Assign ports

Let Docker assign any ports it needs (within 49153 to 65535):

	docker run -P my_image_name

Specify the ports to assign:

	docker run -p 5000:5000 my_image_name

Let Docker assign a port on `localhost`:

	docker run -p localhost::5000 my_image_name


## Naming containers

	docker run --name my_container_name my_image_name


### Linking

Use the name for linking containers:

	docker run --link my_container_name:my_alias --name my_new_container my_image_name

This adds an entry to `/etc/hosts` like `127.0.0.1 my_alias`.
This is updated between restarts.

It also creates environment variables prefixed with `MY_ALIAS_`.
These are not updated between restarts, so hosts is better.
