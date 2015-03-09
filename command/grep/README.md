# grep

Search file contents using a Regular Expression and print matching
lines.


## Search for a pattern in a file

	grep "my_pattern" my_file.txt


## Recursive search

Search in all folders recursively from the current one.

	grep -r "my_pattern" .
	grep --recursive "my_pattern" .


## Search options

Ignore case: `-i` or `--ignore-case`

Invert (show non-matching): `-v`, `--invert-match`

Multiple patterns: `-e PATTERN`, `--regexp=PATTERN`

Stop after count: `-m NUM`, `--max-count=NUM`


## Output options

Print lines before match: `-B NUM`, `--before-context=NUM`

Print lines after match: `-A NUM`, `--after-context=NUM`

Print match count instead: `-c`, `--count`


## Links

- [grep on Wikipedia](http://en.wikipedia.org/wiki/Grep)
