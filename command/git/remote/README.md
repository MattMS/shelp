# git remote

Remotes are copies of your repository that exist in other locations.
They are completely independent and may have different changes applied.

If you used `git clone` to get your repository, then you will have a
remote called `origin` that points to where you cloned from.

You use git [pull](../pull/) and [push](../push/) to receive and send
changes at a remote.


## Print remote names

	git remote


## Print remote names and URLs

	git remote -v


## Add a new remote

	git remote add my_remote git@github.com:MattMS/shelp.git


## Update the URL of a remote

	git remote set-url my_remote git@github.com:MattMS/shelp.git


## Rename a remote

	git remote rename my_old_remote my_new_remote


## Delete a remote

	git remote remove my_remote
