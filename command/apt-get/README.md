# apt-get

These commands will need to be run as root, so prefix with `sudo`.

Package locations are stored in `/etc/apt/sources.list`.


## Install a package

	apt-get install my_desired_package

Installs dependencies of the specified package.
Provides the list of dependencies for confirmation before installing
them.


## Update information about known packages

	apt-get update


## Update all packages and remove unused ones

	apt-get dist-upgrade


## Update all packages but do not remove unused ones

	apt-get upgrade
