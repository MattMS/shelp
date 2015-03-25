# git rebase

If your `git push` fails, you probably want to use `git rebase`.

Assuming you are on `master` branch:

    git fetch origin master
    git rebase origin master
    git push

This will apply your local commits after those from `origin`.
