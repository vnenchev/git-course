# 44 Fast forward vs real merges

- two types of merges - fast forward and real merge
- FAST FORWARD MERGE - no new commit is created git moves the commits from the other branch and that's it
- if you have branch you want to merge to main but main doesn't have other forward commits only the split commit then you have fast forward merge because main is just being continued with the other branch
- when you have fast forward merge no new commit is created, just your commits from the leading branch are incorporated into receiving branch
- REAL MERGE
when you have real merge a new merge commit is created, this commit has two parents