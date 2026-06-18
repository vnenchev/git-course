# 91 Blame

- debugging tool which browse annotated version of a file
- the annotations show which commits changed what lines in the file
- useful for probing the history behind a file's contents
- useful for identifying which commit introduced a bug
- `git blame filename.txt`
- `git blame index.html`
- annotations are on the left side, content of the file is on the right
- navigation is arrows and space bar to do down one page and q to quit
- `git blame -w filename.txt` - ignore any white space changes
- `git blame --date=short filename.txt` - customize the date format
- `git blame -s filename.txt` - suppress commit author and date completely, much shorter annotations
- `git blame --color-lines filename.txt` - will change the color of the line when a line was affected by a different commit then the line before it
- `git blame -L 100,125 filename.txt` - range of lines
- `git blame -L 100,+25 filename.txt` - starting line and how many lines to show
- `git blame d9dba1 filename.txt` - by default the current HEAD is used but you can specify a commit you want