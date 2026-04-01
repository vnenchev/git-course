# 24 Revert commit

- Revert: return to a previous state it is like flipping the commit as if it has never been done
- it is literally undoing changes we made in the past
- reversing or undoing a commit in the repository
- `git revert abc123`
- git adds a new commit to the repo that reverses the specified commit
- may encounter conflicts if simple reversal is not possible, therefore atomic commits are very good because small changes
- `git show --color-words abc123` - to see the exact changes colored
- you auto get text `This reverts commit abc123`
- still if the reverted file was modified later than the commit in question there are still possible conflicts
- in this case you will be asked in what way should the commit be reversed
- this is the place where if your commits are small and focused you will see the benefits