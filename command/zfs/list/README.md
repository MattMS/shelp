# zfs list

## List ZFS snapshots

	zfs list -t snapshot


## Sorting

Print datasets from most to least space used:

	zfs list -S used

Print from oldest to newest creation time:

	zfs list -s creation
