# 68 Delete a remote branch

- deletes the branch from the remote repository - Github
- deletes your remote tracking branch your local tracking remotes branch
- doesn't delete any other local branches
- doesn't change collaborator repositories
- useful when a feature branch is complete and merged
- `git branch feature` to create local branch
- `git branch -d feature` to delete local branch
- `git push -d <remote> <remote-branch>` to delete remote branch
- `git push -d origin feature`
- the branch is now deleted for you but not for your collaborators it is called stalled branch