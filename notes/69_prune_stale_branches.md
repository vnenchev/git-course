# 69 Prune stale branches

- delete all stale branches
- stale branch: a remote-tracking branch that no longer tracks anything because the actual branch in the remote repository has been deleted
- remote branches are three types:
    - branch on the remote repository (bugfix)
    - local snapshot of the remote branch (origin/bugfix) remote tracking branch
    - local branch, trackign the remote branch (bugfix) through origin/bugfix
- when you are deleting a remote branch it deletes your remote-tracking branch too, but not for your collaborators
- fetch doesn't delte remote-tracking branches by default
- so you need to manually prune your remote-tracking stalled branches
- `git remote prune origin` => origin here is the name of the remote, this is usually the defualt
- `git remote prune origin --dry-run` to see what will be removed
- you can prune while fetching => `git fetch --prune` or `git fetch -p`