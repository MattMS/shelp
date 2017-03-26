# mkfifo

Created a named pipe:

	mkfifo my_pipe
	gzip -9 -c < my_pipe > out.gz &

Send data to the pipe:

	cat my_file > my_pipe

Remove the pipe:

	rm my_pipe


## Links

- [Named pipe @ Wikipedia](https://en.m.wikipedia.org/wiki/Named_pipe)
