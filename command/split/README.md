# split

Split a single file into multiple files.

	split my_file my_file_parts

The second argument is the prefix of the parts.

Default size is 1000 lines, with parts prefixed is "x".


## 50 line files

	split -l 50 my_file
	split --lines=50 my_file


## 1024 byte files

	split -b 1024 my_file
	split --bytes=1024 my_file
