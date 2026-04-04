# 34 Format the commit log

- `git log --format=fuller`
- `--format=` option has many different options `oneline, short, medium, full, fuller, email, raw`
- `git log -p` is not only showing commits but also diff for them, -p stands for patch, same as using `git show` for every commit
- `git log --stat` => statistics overview of what was changed
- `git log --graph --all --oneline --decorate` > very useful representation of all commits and all branches
- very useful are `git log -p` and `git log --stat`
- there is also `git log --graph` but it is useful when you have branches