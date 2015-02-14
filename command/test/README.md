# test

Test files types and details.

```fish
if test -d my_folder
	echo "Is folder"
end
```


## Options

- File is not empty (size not 0) with `-s`

- Path exists with `-e`


### Permissions

- Executable file with `-x`

- Readable file with `-r`

- Writable file with `-w`


### Types

- Folder with `-d`

- Regular file with `-f`

- Symbolic link with `-L`
