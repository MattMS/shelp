# zoneadm list

## Zone names

	zoneadm list

Each name is on a new line.


## Configured zones

	zoneadm list -cv

`-c` includes configured zones.
`-v` provides extra output.


## Zone details in CSV

	zoneadm list -p

Each zone is on a new line.
Values are separated by colons (:).

Values are:

- ID number

- Zone name

- Status

- Path

- UUID

- Brand

- IP
