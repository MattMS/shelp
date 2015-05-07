# git log

Print details of commits on current branch.


## Default paging

	git log

Each entry shows the commit ID, author, date and message.

Opens the log in a pager (like [less](../../less/)) if it takes up more
than one screen.


## View commits as one line

	git log --oneline

Same paging as `git log` but only uses one line per commit.

Prints the start of the commit ID and the first line of the message.


## Limit commits

	git log -n 2

Only shows the last 2 commits.


## Links

- [Main docs](https://git-scm.com/docs/git-log)
