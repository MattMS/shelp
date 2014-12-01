# gzip

Compress `my_file` to `my_file.gz` and delete the original:

	gzip my_file

Opposite of [gunzip](../gunzip/).


## Keep original file

	gzip -k my_file

Or

	gzip --keep my_file


## List compression details

	gzip -l my_file.gz

Or

	gzip --list my_file.gz

Lists compressed and uncompressed sizes, compression ratio and original
name.


## Compress each file in a folder

	gzip -r my_folder

Or

	gzip --recursive my_folder

This creates a compressed file for each file found.
