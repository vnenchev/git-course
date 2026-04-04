# 31 The HEAD pointer

- The HEAD pointer references to the tip of the current branch in repository
- points to the parent of the next commit, where writing new commits will occur
- it is the most recently stored state of the current branch
- alternatively you can call it most recently stored state of the current branch
- the HEAD pointer represents your current location inside the repository, if you switch branch the HEAD moves to tip of that branch
- it is always the position when we write the next commit
- the HEAD is maintained in a file => `ls .git` look for a file called HEAD => .git/HEAD => refs/heads/main => .git/refs/heads/main there you will find the SHA of the last commit
- this file points to another place `.git/refs/heads` and inside you will find records for each branch you have
- for example you can have `git diff 3jkl34..HEAD`
- if you switch the branch the HEAD moves to the tip of the new branch
- you have symbolic links for : local branches / remote branches / tags
- symbolic links are maintained by the command `git symbolic-ref`