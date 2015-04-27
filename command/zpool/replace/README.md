# zpool replace

Replace the old device with a new device.

	zpool replace my_pool my_old_device my_new_device

The size of the new device must be at least as large as the minimum size
of all devices in the mirror or raidz configuration.

Leaving off "my_new_device" will use "my_old_device".
This is useful if the device has been physically replaced.
