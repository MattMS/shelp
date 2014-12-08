# scp

Copy files from/to hosts via ssh. 

## Copy from REMOTE host to LOCAL host

	scp my_user@mydomain.com:foo.txt /some/local/directory 

This will prompt for the password for `my_user`.


## Copy from LOCAL host to REMOTE host

	scp foo.txt my_user@mydomain.com:/some/remote/directory

This will prompt for the password for `my_user`.



