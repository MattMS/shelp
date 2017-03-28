# curl

Download content from the Internet.

Alternative to `wget`.


## Availability

Not included in Alpine Linux.


## Download content

Print to `stdout`:

	curl http://example.com/index.html

Save a file:

	curl http://example.com/ > index.html


## HTTP methods

Method names must be specified in uppercase!

Delete all documents in Elasticsearch:

	curl --request DELETE http://localhost:9200/my_index/my_document_type/

or

	curl -X DELETE http://localhost:9200/my_index/my_document_type/


## Print HTTP headers and content (-i)

	curl -i http://example.com/index.html

First line should be `HTTP/1.1 200 OK` if the request worked.


## Send data with request (-d)

	curl -d '{"my_var":["a_string"]}' http://example.com/
