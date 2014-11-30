# Commands

## Navigate the file system

- [cd](./cd/) to change folder.

- [ls](./ls/) to show contents of the current folder.

- [popd](./popd/) to return to the folder saved with `pushd`.

- [pushd](./pushd/) to save the current folder and move to another.

- [pwd](./pwd/) to print which folder you are in.

- [pwdx](./pwdx/) to print which folder a process is in.


### Search by name or contents

- [find](./find/) to search by file name or other attributes.

- [grep](./grep/) to search by file contents.

- [which](./which/) to show if and where the command is installed.


## Modify the file system

- [cp](./cp/) to copy files.

- [ln](./ln/) to create a link to a file or folder.

- [mkdir](./mkdir/) to create a folder.

- [mv](./mv/) to rename or move a file or folder.

- [touch](./touch/) to create an empty file.

- [rm](./rm/) to delete files or folders.

- [rmdir](./rmdir/) to delete an empty folder.


### File and folder security

- [chgrp](./chgrp/) to change the group a file or folder belongs to.

- [chmod](./chmod/) to change permissions of a file or folder.

- [chown](./chown/) to change owner and group of a file or folder.


## View file contents

- [cat](./cat/) to print the full contents of files.

- [diff](./diff/) to get line differences between text files.

- [echo](./echo/) to print a line of text.

- [head](./head/) to print the first 10 lines of a file.

- [less](./less/) to open a file content viewer.

- [tail](./tail/) to print the last 10 lines of a file.


## Modify file contents

- `ed`

- `nano` is a basic text editor.
  Useful for editing single files.

- `sed`

- [tee](./tee/) to save a copy of the given file.

- `vim` is a general text editor.
  Useful for editing single or multiple files.


### File compression tools

- `gunzip`

- `gzip`


## View resources

- [free](./free/) to print memory usage.


### View disk space

- [df](./df/) to print how much disk space is free.

- [du](./du/) to print the disk usage (size) of files or folders.


### View processes

- `ps`

- [top](./top/) to open a process resource monitor.


## Modify processes

- `kill`


## Manage packages

- [apt-cache](./apt-cache/) to print package details.

- [apt-get](./apt-get/) to install packages.


## Networking tools

- `ip`

- `ping`
