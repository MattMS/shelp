# fuser

Print processes using a specific file:

	fuser /etc/passwd

If there are no users, it will print the file name and a colon (:).

If there are users, it will add the process ID to the end, with a letter
indicating what state the process has the file open in.


## Links

- [illumos man page](http://illumos.org/man/1m/fuser)
