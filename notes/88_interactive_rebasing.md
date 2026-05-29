# 88 Interactive rebasing

- Give us a change to modify commits as they are being replayed
- opens the git-rebase-todo file for editing and wait for us to do the editing
- car reorder or skip commits
- can edit commits contents
- git provides the plan but lets you edit the plan
- interactive rebase choices:
    - pick, drop => use it or dont use a commit
    - reword, edit => reword the commit message or edit the change set
    - squash, fixup => several commits into one
    - exec => runs a command from the shell, advanced feature which is rarely used
- `git rebase -i <upstream> <branch>`
- `git rebase -i main new_feature`
- commit line starts with `pick` but down you will find the description for each command
- you can also edit commit without moving them to a new merge base `git rebase -i HEAD~3` so you can recommit the commits on the current branch instead of doing reset
- don't forget that it is destructive and is useful for local branches with not many commits
- the above rebase the branch several commits in the past on the same branch
- it picks the last three commits and give you opportunity to edit them
- to undo rebase you need the merge-base SHA and use `git rebase -i --onto=<old_merge_base SHA> main`