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

- [create](./create/) a new pool.

- [destroy](./destroy/) a pool.

- [export](./export/) a pool with unmounted devices.

- [import](./import/) pools, or list importable pools.

- [scrub](./scrub/) to verify data checksums are correct.

- [split](./split/) mirrored disks into a new pool.

- [upgrade](./upgrade/) to view current and possible versions.


### Devices

- [add](./add/) a device to the pool.

- [clear](./clear/) device errors in a pool.

- [offline](./offline/)

- [online](./online/)

- [remove](./remove/) a device from a pool.

- [replace](./replace/) old device with a new one.


### Mirrored devices

- [attach](./attach/) a device to a mirrored device.

- [detach](./detach/) a device from a mirrored pool.


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


## Links

- [illumos man page](http://illumos.org/man/1m/zpool)
