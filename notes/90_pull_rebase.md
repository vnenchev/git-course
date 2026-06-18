# 90 Pull rebase

- fetch from remote, then rebase instead of merging -> git pull does fetching than merging which is different
- `git pull -r` or `git pull --rebase`
- it will rebase your commits instead of merging
- keeps history cleaner by reducing merge commits
- only use on local commits not shared to a remote
- if you are working on feature branch and in the mean time main has advanced you fetch the commits and if you have just a few commits in your feature branch you can easily integrate them into your main without causing trouble
- if you provide `git pull --rebase=preserve` - to preserve locally created merge commits and not flatten them when doing rebase
- if the commits you're rebasing includes some merge commits, then you probably want to use preserve to keep the exact history
- if you provide `git pull --rebase=interactive` uses the interactive rebasing technique from above
- if you do git pull -r then your changes are rebased after the fetched changes from the remote
- example for collaborator that is pretty much out of sync is to do `git reset --hard origin/main` , that way he/she is catching up the changes