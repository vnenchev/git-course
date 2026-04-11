# 45 Resolve merge conflict

- if you try to merge two branches with overlapping changes you have merge conflict
- you can try to simulate that by doing conflicting commits and trying to merge them
- dont forget to view the graph `git log --graph --all --oneline --decorate`
- if you have merge conflict your prompt changes to for example (main|MERGING)
- the conflicts are marked with >>>>> and <<<<<< symbols
- the resolve is in the next chapter for now if you just want to abort use `git merge --abort`
- to check if conflicting files `git status` or `git ls-files -u`
- `git log --merge --left-right -p`