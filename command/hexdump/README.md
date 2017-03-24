# hd, hexdump

Displays the contents of a file as columns of hex data.
Each line represents 16 bytes.
The first column is the offset, as a hex value.
The remaining 8 columns of 4 hex characters each represent 2 bytes.

Use `-v` to stop duplicate lines being displayed with `*`.


## Restrict range (limit, skip)

To ensure only 64 bytes are displayed (4 lines):

	hexdump -n 64 my_file

To also skip the first 16 bytes (1 line):

	hexdump -n 64 -s 16 my_file


## Alternate output formats

To display each 2 byte column as decimal numbers:

	hexdump -d my_file

Display 16 1-byte hex columns with 1 16-byte ASCII column at end:

	hexdump -C my_file

There is also support for specifying custom formats with `-e` and `-f`.
