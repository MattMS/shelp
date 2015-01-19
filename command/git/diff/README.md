# git diff

Git diff prints the added, changed and removed lines in files.

If there are more lines than will fit in the terminal, then a pager will
be used to let you scroll through the changes.
You can press `q` to quit the pager.


## View changes of all unstaged files

	git diff


## View changes of a single unstaged file

	git diff my_file


## View all staged changes

	git diff --cached
