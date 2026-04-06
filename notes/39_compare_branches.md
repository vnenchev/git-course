# 39 Compare branches

- `git diff main..mynewbranch` beware that the first branch is taken as older and put into the minus side
- if you want to know only the changes in the mynewbranch branch and not in the main branch use:
- `git log --graph --all --on --decorate` to see where do the branches split and compare from there
- the point where branches split off is called `the merge base` , you can also find it with `git merge-base main mynewbranch`
- with merge base you can find the difference only for the branch in question very useful
- maybe you are working with collaborator and want to see only their changes and then can use the technique from above
- the command `git checkout -m branch_to_receive_changes`is trying to merge your changes with the branch you