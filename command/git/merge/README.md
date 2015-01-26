# git merge

Merge another branch into your current branch.

Since git knows the current branch you are in, the name you give to
`merge` is the branch you want to get changes from.


## Basic merge

	git checkout master
	git merge develop

`git checkout master` changes the current branch to `master`.
`git merge develop` merges the `develop` branch into your current branch
(`master`).
