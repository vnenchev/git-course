# 48 Soft reset

- moves branch and HEAD pointer
- does not change staging index
- does not change working directory
- `git reset --soft <commit>`
- `git fsck --unreachable` it shows you all of the unreachable items or commits left as orphan
- change the repository state and leave all changes in staging index
- useful for amending one or more commits this is the most frequent use case
- roll back the history and everything again
- similar to `git commit --amend` but done for more than just one commit
- SHAs for commits will change
- if you don't have any commits after the soft reset you can go to whichever commit you like, no pending changes, reset as much as you like