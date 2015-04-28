# zpool list

Print pools and health status.

	zpool list

Lists all pools if no parameters are given.


## Health

- "DEGRADED": some failed devices but data is still available.

- "ONLINE": all devices operating normally.

- "SUSPENDED": waiting for a device issue to be resolved.

- "UNAVAIL": failed or corrupted devices preventing usage.
