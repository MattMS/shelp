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

- allow

- create

- destroy

- diff

- [help](./help/) to print information on subcommands.

- key

- mount

- rename

- share

- unallow

- unmount

- unshare

- upgrade


### Clone

- clone

- promote


### Properties

Native properties control ZFS behaviour.

User properties can be used to annotate datasets.
They have no effect on ZFS behaviour.

- [get](./get/)

- inherit

- [list](./list/) to print property information.

- [set](./set/)


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
