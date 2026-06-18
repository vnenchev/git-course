# 84 Create formatted patches

- if you compare with diff patches they don't have history and everything is smushed into single file, here you have options
- export each commit in unix mailbox format, useful for email distribution of changes
- include changes, commit messages and some metadata
- one commit per file by default
- `git format-patch 2e33d..655da` create formatted patch from a range of commits
- `git format-patch -1 655da` - create formatted patch for a single commit
- if we are creating mini files, we probably want to put them somewhere besides in our current directory.
- `git format-patch 2e33d..655da -o feature_patches` -o for output and directory to store it
- trick to output to a single file `git format-patch 2e33d..655da --stdout > feature.patch`
- it tells you the name of the created files and status, they have numbers in front because order is important