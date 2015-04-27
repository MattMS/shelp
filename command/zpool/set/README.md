# zpool set

Set a property on a pool:

	zpool set my_property=my_value my_pool


## Properties

### Any time

Can be set at creation or import time.
Can be changed later with `zpool set`.

- autoexpand

- autoreplace

- bootfs

- cachefile

- dedupditto

- delegation

- failmode

- listshares

- listsnaps

- version


### Creation time

Can be set at creation or import time.

- altroot


### Import time

- readonly
