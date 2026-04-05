# 36 Create branches

- `git branch` gives you a list of all branches
- the `*` asterisk in front of the branch name indicates that we are on that branch at the moment
- the dot next to the name of the branch indicates that the head is on this branch
- to create branch `git branch mynewbranch` or also `git switch -c mynewbranch` or also `git checkout -b mynewbranch` fails if branch exists, and if picking particular commit `git branch mynewbranch v1.5` here important is if you have tags or other way to point to the particular commit
- you can also use `git checkout -B mynewbranch` - to create a new branch forcefully
- be very careful with `git checkout -B mynewbranch` because it already exist it will be overwritten by the current branch
- you can try to create hierarchical naming system like `mainbranch/otherbranch mainbranch/somebranch` and now you are able to search within these names because of Unix feature called masks - `git show branch 'mainbranch/*'`
- command `git show-branch` , upper part every branch is indicated with ! and color coded and the current branch is indicated with `*`, the below part is showing: asterisk for the current branch, `+` if the commit is present in this branch and minus if the merge is successful