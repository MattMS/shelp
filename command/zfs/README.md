# zfs

`zfs` configures ZFS datasets within ZFS pools.


## Dataset types

### filesystem

Behaves mostly the same as a POSIX filesystem.
May fail when checking free file space.

This is the most commonly used dataset type.


### snapshot

Read-only version of the filesystem.


### volume

Logical volume exported as a raw or block device.
Only used under special circumstances.


## Subcommands

- [create](./create/) a filesystem or volume.

- [destroy](./destroy/) a filesystem or snapshot.

- [diff](./diff/)

- [help](./help/) to print information on subcommands.

- `rename` to rename a dataset, share or snapshot.

- `upgrade` identifies the filesystem version.
  Add `-a` to perform the upgrade.


### Clone

- [clone](./clone/) a snapshot of a dataset.

- `promote` a cloned filesystem to remove the snapshot dependency.
  This allows the original snapshot to be deleted.


### Mounting filesystems

- `mount` to show mounted filesystems or mount a new one.

- `unmount` to unmount a filesystem.


### Properties

Native properties control ZFS behaviour.

User properties can be used to annotate datasets.
They have no effect on ZFS behaviour.

- [get](./get/)

- inherit

- [list](./list/) to print property information.

- [set](./set/)


### Security

Grant permissions to other users for administering ZFS file systems in a
storage pool.
Generally the ability to use a subcommand or change a property.

- allow

- [key](./key/) to create, change or load/unload a dataset key.

- unallow

	man zfs_allow
	man zfs_encrypt


### Share

- share

- unshare

	man zfs_share


### Snapshot

- hold

- holds

- release

- rollback

- snapshot


### Space

- groupspace

- userspace


### Stream

- receive

- send


## Links

- [illumos man page](http://illumos.org/man/1m/zfs)
