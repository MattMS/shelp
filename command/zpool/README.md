# zpool

`zpool` will throw an error requesting a command.

`zpool` does not take into account space used by ZFS internally, but
[zfs](../zfs/) does.


## Help

List subcommands:

	zpool help

List "add" subcommand usage options (no descriptions):

	zpool help add


## Subcommands

- [create](./create/)

- [destroy](./destroy/)

- [export](./export/)

- [history](./history/)

- [import](./import/)

- [iostat](./iostat/)

- [list](./list/)

- [scrub](./scrub/)

- [split](./split/)

- [status](./status/)

- [upgrade](./upgrade/)


### Devices

- [add](./add/)

- [attach](./attach/)

- [clear](./clear/)

- [detach](./detach/)

- [offline](./offline/)

- [online](./online/)

- [remove](./remove/)

- [replace](./replace/)


### Properties

- [get](./get/)

- [set](./set/)


## Virtual devices (vdevs)

A zpool is a collection of virtual devices.

Virtual devices cannot be nested.
A "mirror" or "raidz" device can only contain disks or files.

Hot spares can be added to come online if an active device fails.


### Device types

Using a full disk is preferred to using parts of a disk.

Using regular files as devices is strongly discouraged.
