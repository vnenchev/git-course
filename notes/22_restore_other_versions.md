# 22 Restore other versions

- as we develop things very often we want to restore to even older version that is already in our repository
- we can pick a version of a file from commit far behind if we want that
- `git restore file.txt --source=6a94c13d` - source is an old commit here or older way `git checkout <source commit> -- <path to file>`
- file will be restored in our working directory
- `git log --oneline`, pick index.html from initial commit `git restore index.html --source=41b1ed`
- check what the changes are with `git diff` and if you don't like the result `git restore index.html` will remove old version and get the new instead
- after `restore` the changes will be in your working directory ready to be added and committed
- Git stores full version of latest files
- this make it very fast with recent changes and not so fast with older changes 
- compared to the other VSC before Git they worked the other way around - applying change sets as we go forward, so they were faster working with older versions and not so fast working with recent versions