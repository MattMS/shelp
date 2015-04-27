# zoneadm list

Prints each zone on a new line.

	zoneadm list -cv


## Status

Only running by default:

	zoneadm list


### Configured and running

	zoneadm list -c


### Installed and running

	zoneadm list -i


## Output style

Default output is only the zone name.

`-p` and `-v` columns are:

- ID number

- Zone name

- Status

- Path

- UUID

- Brand

- IP


### Table (verbose)

	zoneadm list -v


### Zone details in CSV

	zoneadm list -p

Values are separated by colons (:).
