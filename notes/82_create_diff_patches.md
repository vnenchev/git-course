# 82 Create diff patches

- patches allows us to export changes into external files
- useful when you want to store a set of changes outside of the repository
- useful when collaborators do not share a remote, then put files on thumb drive or hard drive to share
- sharing patches was more popular before git and remote repositories
- can be used during, discussion, review, approval process
- `git diff from-commit to-commit > output.diff`
- `git diff origin/main..main > output.diff