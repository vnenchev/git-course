# 49 Mixed reset

- moves branch and HEAD pointer
- Changes staging index to match repository
- doesn't change the working directory
- mixed reset is the default reset `git reset --mixed <commit>` equivalent to `git reset <commit>`
- it is not destructive unless you make other commits after that
- MOST USEFUL FOR REARRANGING COMMITS
- with mix reset if you want you can create branch for commits that is going to be orphaned to not loose track of it
- the resulting branch will be discontinued but reference to it will still exist and later you can use it if necessary
- git branch before_reset => create it and don't switch to it yet, do a `git reset --mixed 32kljkl` on your reset branch
- track your changes with `git log --oneline -5` /or more/ or `git log --graph --all --oneline --decorate`
- now even when you continue your reset branch the before-reset branch still exists