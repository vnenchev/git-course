# 80 Cherry picking commits

- share code between branches and repositories
- cherry picking is the ability to apply one or more existing commits into a new place
- each commit targeted will become a new comiit on the current branch
- conceptually similar to copy and paste
- new commits will have different SHAs but the same changes, commit message and author
- lets assume you have two branches you have a particular commit on the first branch that you want but you don't want the rest of the commits after that just yet
- `git cherry-pick d4e8411d` for a particular commit
- you can also cherry pick range of commits - `git cherry-pick d4e8411d..57d290ec`
- lets investigate commits `git log --oneline --graph --all --decorate`
- `git switch -c new_feature HEAD` - source for new branch the current branch HEAD position
- `git cherry-pick eba078` here eba078 is SHA for the commit from other branch
- and now you have new commit with its own SHA
- look `git --oneline -5`
- you can cherry-pick commits from any branch and that includes remote tracking branches
- you can not cherry pick a merge commit
- by default git will keep previous commit message but can edit it with `git cherry-pick --edit d4e84`
- may result in conflicts that must be resolved