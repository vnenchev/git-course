# 52 View stashed changes

- `git stash list` list all of your stashed items
- `git stash show <stash>` - reference to your stash entry, it is just meta info
- `git stash show -p <stash>` - p stands for patch and show details
- `git stash show -p --color-words 1` even better with highlighting only the change in color
- `git stash show 2` - here 2 is the stack position starting from 0 so it is the third stash
- `git stash show -p 1` - it is showing diff like representation for item 1