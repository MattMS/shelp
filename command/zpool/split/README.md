# zpool split

Split a mirrored disk off each device in a pool and create a new pool
with them.

	zpool split my_pool my_new_pool

The device must not be in the process of resilvering.

Include a device to limit the split.

	zpool split my_pool my_new_pool my_device
