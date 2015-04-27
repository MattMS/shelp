# zpool scrub

Verify the checksums are correct on all data in the pool.
Resilvering only checks known out-of-date data.

	zpool scrub my_pool

Displays progress as it is working and then a summary at the end.

Since it is IO intensive, only one process can occur at a time.

Automatically fixes errors in replicated (mirror, raidz) devices.


## Stop scrubbing

	zpool scrub -s my_pool
