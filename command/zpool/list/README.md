# zpool list

Print pools and health status.

	zpool list

Lists all pools if no parameters are given.


## Health

- "DEGRADED": some failed devices but data is still available.

- "ONLINE": all devices operating normally.

- "SUSPENDED": waiting for a device issue to be resolved.

- "UNAVAIL": failed or corrupted devices preventing usage.


## Select properties to show

This is the default selection:

	zpool list -o name,size,allocated,free,capacity,dedupratio,health,altroot

Names of properties are in [zpool get](../get/).
