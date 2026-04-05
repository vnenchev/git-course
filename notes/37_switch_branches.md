# 37 Switch branches

- `git switch mynewbranch` to switch to the branch, also old way is `git checkout mynewbranch`
- to see references use `cat .git/HEAD` => `refs/heads/mynewbranch`, look here to find out what is the current branch
- edit to the about page to see the differences
- if a branch has not catched up with your current branch, you wont see its tip shown by `git log` or other commands
- when you switch to main branch to new commit on `mynewbranch` is not even shown, because it is not in the history of main branch
- so as you see when you switch branches the files change accordingly to represent the current branch
- to create a new branch and immediately switch to it in one step `git switch --create otherbranch` or `git switch -c otherbranch`