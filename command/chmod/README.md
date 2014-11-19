# chmod

Change the user access permissions on a file.


## Setting permissions with numbers

Permissions can be set with a 3 digit octal number.

- 4 is read

- 2 is write

- 1 is execute/run

- 0 is no permissions

These are added together to given the permission type.

The 3 digits represent owner, group and everyone else.

So `740` lets the owner do anything, users in the file group read it and
everyone else has no access.


## Modifying permissions

They user type must be specified:

- `u` for the owner of the file.

- `g` for users in the file's group.

- `o` for everyone else.

- `a` is the same as `ugo`.


The modification type is then given:

- `-` removes the permission.

- `+` allows the permission.


Then the permission type is given:

- `r` for read access.

- `w` for write access.

- `x` for execution/run access.
  When applied to a folder, this allows a user to open it.


## Give full permissions to everyone for a file

	chmod 777 my_file


## Allow the owner to run a script

	chmod u+x my_script

The script can then be run with:

	./my_script


## Links

[chmod on Wikipedia](http://en.wikipedia.org/wiki/Chmod)
