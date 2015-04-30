# git stash

Save changes since the last commit.

This is useful if you want to change branches without needing to commit
your current changes.


## Save current changes

	git stash save


## Apply changes

	git stash apply

To apply then delete the stash, use `pop` instead of `apply`.


### Create new branch

	git stash branch my_new_branch

Creates the new branch `my_new_branch` and applies the last stash.
Drops the stash after this.


## View

### List of stashes

	git stash list


### Single stash diff

Shows diff between previous commit and the stash contents.

	git stash show

Accepts all `git diff` parameters.
