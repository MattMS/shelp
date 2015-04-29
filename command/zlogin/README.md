# zlogin

Enter a zone.

This can only be used in the global zone.


## Interactive

	zlogin my_zone_name

Performs a normal login for interactive command entry.


## Non-interactive

This is done if a utility is specified (`pwd` in this case).

	zlogin my_zone_name pwd

It exits (with status) once the command is finished.


## Non-root user

	zlogin -l my_user_name my_zone_name

If a user name is not provided then the user is `root`.


## Safe login

This is useful if other login types have failed.

	zlogin -S my_zone_name

This can only be done as `root` and not to a zone console (`-C`).
It does not invoke `login` or `su`.


## Links

- [illumos man page](http://illumos.org/man/1/zlogin)
