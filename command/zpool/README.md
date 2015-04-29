# zpool

Configure ZFS storage pools.

`zpool` does not take into account space used by ZFS internally, but
[zfs](../zfs/) does.

Without arguments, it will throw an error requesting a command.


## Help

List subcommands:

	zpool help

List "add" subcommand usage options (no descriptions):

	zpool help add


## Subcommands

- [create](./create/)

- [destroy](./destroy/)

- [export](./export/)

- [import](./import/)

- [scrub](./scrub/)

- [split](./split/)

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


### View information

- [history](./history/) for a list of commands run.

- [iostat](./iostat/) for storage capacity and usage.

- [list](./list/) for pool health.

- [status](./status/) for detailed health.


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
