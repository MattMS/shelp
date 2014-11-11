# find

The slash (/) at the start of each command means that searching will
start from the root directory.
This means the entire file-system will be searched.


## Search for file name

	find / -name "my_file_name"


## Search for file extension

	find / -name "*.txt"


## Search by file type

	find / -type f

`-type` can be:

- f: regular file

- d: directory

- l: symbolic link

- c: character devices

- b: block devices


## Search by file size

	find / -size 50c

`-size` can be:

- c: bytes

- b: 512-byte blocks

- k: Kilobytes

- M: Megabytes

- G: Gigabytes


## Search by owner, group or permission

	find / -user root

	find / -group shadow

Must have the given permission:

	find / -perm 644

Must have at least the given permission:

	find / -perm -644


## Save/ignore errors while searching

Save errors to `errors.txt`:

	find / -name "my_file_name" 2>errors.txt

Ignore errors:

	find / -name "my_file_name" 2>/dev/null


## Links

- http://www.codecoffee.com/tipsforlinux/articles/21.html

- https://www.digitalocean.com/community/tutorials/how-to-use-find-and-locate-to-search-for-files-on-a-linux-vps
