# od

Display file contents in octal format.
Each line represents 16 bytes.
The first column is the offset, as an octal value.

`od` has a similar output to [hexdump](../hexdump/), but flags are different.


## Restrict range (limit, skip)

To ensure only 64 bytes are displayed (4 lines):

	od -N 64 my_file

To also skip the first 16 bytes (1 line):

	od -j 16 -N 64 my_file


## Alternate output formats

Change offset column format to hex:

	od -A x my_file
