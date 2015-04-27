# zoneadm mark

Change the state of a zone.

	zoneadm -z my_zone mark incomplete


## States

### incomplete

Useful if a zone is unusable.

This cannot be undone, except by uninstalling the zone.


### unavailable

Useful if a zone is unusable.

This can be undone with [attach](../attach/).
