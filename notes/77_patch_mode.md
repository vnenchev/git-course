# 77 Patch mode

- select portioin of a file to stage, very useful if several changes in the same file but not directly related
- "Hunk" : an area of a file with a group of changes
- Hunks can be staged, skipped, or split into smaller hunks
- `git add -i` to go to interactive mode
- choose 5 or p for patch, select the file to patch
- select the file and see the letter options "y,n,q,a,d,j,J,g,/,s,e,p,?"
- also accesssible from the command line with `git add -p` or `git add --patch`
- patch is used in git stash, git restore, git reset, git commit