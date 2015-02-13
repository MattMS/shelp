# awk

Line-based text processing language.

Each line is a "record" and each word is a "field".

Commands take the form:

	condition { action }


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


## Examples

Print lines with more than 80 characters:

	length($0) > 80


## Links

- [AWK on Wikipedia](https://en.wikipedia.org/wiki/AWK)
