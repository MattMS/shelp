# nc (netcat)

Listen for or launch TCP/UDP connections.

Busybox includes `awk`, thus Alpine Linux does.


## Port scan

Check if localhost port 80 is open:

	nc -vz 127.0.0.1 80

Nothing will be shown without verbose output (`-v`).


## Simple TCP connection

In one terminal, start a server on port 1337:

	nc -l 1337

In another terminal, connect to the server:

	nc 127.0.0.1 1337

Typing in either terminal and pressing Enter will show the message in the other terminal.
This can be terminated by EOF (^D) or Ctrl+C (^C).


## Links

- [netcat @ Wikipedia](https://en.m.wikipedia.org/wiki/Netcat)
