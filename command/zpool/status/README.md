# zpool status

Display detailed health status of all pools in the system:

	zpool status

Limit status to a single pool:

	zpool status my_pool

Use `-x` to limit status to pools with errors or unavailable.


## Health

- "DEGRADED": checksum or IO errors exceeds acceptable level.

- "OFFLINE": device was specifically taken offline.

- "ONLINE": functioning normally.

- "REMOVED": device was physically removed.
  Reattaching the device should bring it back "online" automatically.

- "UNAVAIL": device could not be opened.
