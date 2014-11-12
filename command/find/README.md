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

- `f` for regular file

- `d` for directory

- `l` for symbolic link

- `c` for character devices

- `b` for block devices


## Search by file size

	find / -size 50c

`-size` can be:

- `c` for bytes

- `b` for 512-byte blocks

- `k` for Kilobytes

- `M` for Megabytes

- `G` for Gigabytes


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
