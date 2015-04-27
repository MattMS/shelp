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

- [add](./add/)

- [attach](./attach/)

- [clear](./clear/)

- [destroy](./destroy/)

- [detach](./detach/)

- [export](./export/)

- [history](./history/)

- [import](./import/)

- [iostat](./iostat/)

- [list](./list/)

- [offline](./offline/)

- [online](./online/)

- [remove](./remove/)

- [replace](./replace/)

- [scrub](./scrub/)

- [split](./split/)

- [status](./status/)

- [upgrade](./upgrade/)


### Properties

- [get](./get/)

- [set](./set/)


## Health

Hot spares can be added to come online if an active device fails.


### Pool

- "Degraded": some failed devices but data is still available.

- "Online": all devices operating normally.

- "Suspended": waiting for a device issue to be resolved.

- "Unavail": failed or corrupted devices preventing usage.


### Device

- "Degraded": checksum or IO errors exceeds acceptable level.

- "Offline": device was specifically taken offline.

- "Online": functioning normally.

- "Removed": device was physically removed.
  Reattaching the device should bring it back "online" automatically.

- "Unavail": device could not be opened.


## Virtual devices (vdevs)

A zpool is a collection of virtual devices.

Virtual devices cannot be nested.
A "mirror" or "raidz" device can only contain disks or files.


### Device types

Using a full disk is preferred to using parts of a disk.

Using regular files as devices is strongly discouraged.
