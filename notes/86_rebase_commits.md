# 86 Rebase commits

- upstream branch is the branch whose tip will become our new base and follows `<branch>` who's commits we want to rebase
- if the branch you want to rebase then you can omit the `<branch>` part
- it forces each one collaborator to take responsibility of the commits
- Take commits from a branch and replay them at another point, most often at the end of another branch
- useful to integrate recent commits without merging
- maintains a cleaner, more linear project history
- ensures feature branch commits apply cleanly
- `git rebase <upstream> <branch>` - the tip of upstream will become our new base, upstream is the receiving branch
- we can rebase to completely different branch
- `git rebase --onto <new-base> <upstream> <branch>`
- `--onto <new-base>` could be any commit we want
- `git rebase --onto ecommerce main new_feature` - rewind new_feature branch to the place where it merges with main branch and rebase those commits on the ecommerce branch
- we can rebase to a specific commit instead of the tip of any branch `git rebase --onto f36de3b1 main new_feature`
- rebasing commits may conflict with existing code
- git pauses rebase before each conflicting commit
- `git rebase --continue`
- `git rebase --skip`
- `git rebase --abort`