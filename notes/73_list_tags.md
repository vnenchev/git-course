# 73 List tags

- `git tag` and `git tag --list` you list all of your tags
- you can filter tags with `git tag -l "v2*"` you can use "\*" as wildcard character, just tag names without annotations
- `git tag -n` shows the tags and the annotations
- a tag is just a reference to a commit, you can use `git diff v1.0..v1.1` or `git show v1.1`
- if you put `git switch v1.1` you get an error because tag is not the same as branch
- you can create new branch from a tag because it is just a reference to a commit `git switch -c branch_v1 v1.0`
- where are tags stored => .git/refs/tags