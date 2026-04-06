# 41 Delete branches

- `git branch -d <branchname>`, you can't delete a branch that you are currently on, and this commands delete the branch if it has been fully merged
- check your current branch with `git branch`, look for the asterisk to understand which is your current branch
- `git switch -c deletionbranch` create deletionbranch and auto switch to it
- deleting branches that have unmerged changes on them `git branch -D deletionbranch` forcefully
- two protections: one is can't delete the branch currently on, two can't delete if unmerged changes exists
- if you type `git branch -d deletionbranch` if there are uncommitted changes it is not possble