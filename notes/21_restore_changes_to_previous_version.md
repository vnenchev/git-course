# 21 Restore changes to previous version

- if file is not staged `git restore <filename>` => also old way is `git checkout HEAD <filename>` and can be found in old code, if working with scripts take a note of this
- if the file is staged `git restore --staged <filename>` for which old way is => `git reset HEAD <filename>` and then `git restore <filename>` to remove the changes from the working directory if you want to completely remove the changes
- to restore everything use `git restore .` 