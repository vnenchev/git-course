# 12 Edit files
- we need to learn how Git notices changes to tracked files and learn how to commit those changes
- make some edits, add lines, now the file is designated as `modified:` when execute `git status` 
- `git show` will show you your modifications
- shortcut for adding and committing at the same time `git commit -am "commit message"`
- beware you cannot put `git commit -am "message"` for untracked files, you need to first `git add <filename>` or `git add .` for the entire directory
- you can commit even if there is still untracked and modified files, they will wait there until an action is taken
- to remove your changes from a file in the working directory use `git restore <file>`
- staged files are typically in green, file in the working directory which are modified are typically red