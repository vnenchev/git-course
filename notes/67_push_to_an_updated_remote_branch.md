# 67 Push to an updated remote branch

- fetch the latest commits from remote branch
- merge into your local branch
- resolve any merge conflicts
- push to the remote branch
- there is Force push
    - replaces remote branch with local branch
    - use if local branch is preferable to remote branch
    - this destroy commits - use with caution
    - this will be disruptive for collaborators using the remote branch
    - force push is `git push -f`, maybe good idea if you know that you are the only developing on this branch