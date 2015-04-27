# zoneadm detach

Detaching is the first step in migrating a zone to another system.
Then the zonepath is moved before the zone is attached.

Zone must be halted before detaching.

	zoneadm -z my_zone detach

Zone is left in a configured state after being detached.

Use `-n` to do a "dry run" (no changes) that can test for issues.
