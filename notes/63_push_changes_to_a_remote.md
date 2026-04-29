# 63 Push changes to a remote

- `git push <remote> <local-branch>:<remote-branch>` => like `git push origin main:main`
if the current branch is setup to track this remote branch, then we don't have to type all of this just `git push`
remind yourself about the current commits with `git log --oneline` look where is the main and origin/main pointers
it is good to know the full command for the advanced cases when it's not a tracking branch or when you want to push from or to a different branch
most of the time you will be using git push
to check the log for a single branch use `git log -5 --oneline main` you can also `git log -5 --oneline origin/main`