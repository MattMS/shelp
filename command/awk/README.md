# awk

Line-based text processing language.

By default, each line is a "record" and each word is a "field".

Commands take the form:

	condition {action}


## Availability

Busybox includes `awk`, thus Alpine Linux does.

Alpine path: /usr/bin/awk


## Print single field

Print first field of second record:

	NR == 2 {print $1}

Print last field of every record:

	{print $NF}

Print second last field of every record:

	{print $(NF - 1)}

Print line count:

	END {print NR}


## Match by function

Print records with more than 80 characters:

	length($0) > 80 {print}


## Match by regular expression

Match entire record:

	/test/ {print}

Match first field:

	$1 ~ /test/ {print}

Inversely, print records with first field *not* matching the regex:

	$1 !~ /test/ {print}


## Writing scripts

Comment line with a hash (#) and join lines with a semicolon (;).

Start an awk script file with `#!/usr/bin/awk -f`.
Invoke it with `./my_script.awk my_data_file.txt`.

Alternatively, replace `-f` with `-E`/`--exec` to prevent further command-line arguments, such as variable assignment (`-v`/`--assign`).
Useful for security in CGI scripts.

Use `-S`/`--sandbox` to prevent access to the system.
Useful for scripts from untrusted sources.


## External scripts

Include an awk script from the command with `-e`/`--source`:

	awk -e my_library.awk -f my_script.awk my_data_file.txt

Include an awk script in the source:

	@include "my_script.awk"
	BEGIN {print "hello"}


## Built-in variables

- `$0` = whole record.

- `$1` = first field.

- `$2` = second field.

- `$NF` = last field.

- `FILENAME` = current file name.


### Current counts

- `NF` = count of fields in record.

- `NR` = current count of records.


### Input separator

- `FS` = field (defaults to whitespace characters).

- `RS` = record (defaults to new line).


### Output separator

- `OFS` = field (defaults to space).

- `ORS` = record (defaults to new line).


## Functions

	function my_func (my_arg) {
		return my_arg + 1
	}

	print my_func(2)


## Example ini file search

`ini_search.awk`:

	BEGIN {FS = "="}
	/^\[.*\]$/ {current_group = substr($0, 2, length - 2)}
	current_group == group && $1 == key {print $2}

Get value of key/property `b` in group/section `[a]`:

	awk -v group=a -v key=b -f ini_search.awk test.ini

**NOTE:** Don't use this for real! It is not a proper ini parser (doesn't ignore comment lines, cuts values containing `=`, probably more wrong stuff).


## Links

- [gawk manual](https://www.gnu.org/software/gawk/manual/gawk.html)

- [7.5 Predefined Variables @ gawk manual](https://www.gnu.org/software/gawk/manual/gawk.html#Built_002din-Variables)

- [AWK @ Wikipedia](https://en.m.wikipedia.org/wiki/AWK)
