# git clone

`git clone` makes a local copy of the specified repository.
You can commit changes and they will not be pushed back into the
original repository until you use `git push`.

	git clone git@github.com:MattMS/shelp.git

This will create a folder called `shelp` that contains the repository.


## Change folder

	git clone git@github.com:MattMS/shelp.git shell_help

Creates the folder `shell_help` instead of `shelp`.

You can rename the folder using [mv](../mv/) and the repository will be
unaffected.
