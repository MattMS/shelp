# tail

Print last 10 lines of a file:

	tail my_file

Or print chosen number of lines:

	tail -n 20 my_file


## Follow and print changes

Print last 10 lines then follow changes to a file:

	tail -f my_file

The `-F` argument works if the file is recreated, renamed or removed.

	tail -F my_file


## Links

- [tail on Wikipedia](http://en.wikipedia.org/wiki/Tail_%28Unix%29)
