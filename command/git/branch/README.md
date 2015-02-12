# git branch

View and manage branches in the current repository.


## Print branches

	git branch

Highlights the active branch.


## Print branches with last commit

	git branch -v

Includes the last commit ID and first line of the message.


## Delete a local branch

	git branch -d my_branch


## Delete a remote branch

After Git 1.7.0:

	git push origin --delete my_branch_on_origin

After Git 1.5.0:

	git push origin :my_branch_on_origin

From [Delete a Git branch both locally and remotely](http://stackoverflow.com/questions/2003505/delete-a-git-branch-both-locally-and-remotely).
