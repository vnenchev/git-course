# 64 Fetch changes from a remote

- we use `git fetch <remote>` , `git fetch origin`, if no origin specified origin is the default `git fetch`
- fetch will retrieve all branches and the commits that go with them
- fetch will update all remote tracking branches so they point to the correct commits
- fetch will update the origin/main branch but not the main branch
- `git pull` is a command that does both `git fetch` and `git merge` together
- but sometimes you don't want to merge immediately if in a middle of something