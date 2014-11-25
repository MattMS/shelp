# curl

Download content from the Internet.

Alternative to `wget`.


## Download content

Print to `stdout`:

	curl http://example.com/index.html

Save a file:

	curl http://example.com/ > index.html


## Print HTTP headers and content (-i)

	curl -i http://example.com/index.html

First line should be `HTTP/1.1 200 OK` if the request worked.


## Send data with request (-d)

	curl -d '{"my_var":["a_string"]}' http://example.com/
