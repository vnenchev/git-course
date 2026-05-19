# 79 Edit a hunk

- most useful when a hunk cannot be split automaticallly
- can edit a hunk manually
- modify a diff of the changes in a text editor
- diff-style line prefixes: +, -, space
- enter mode from git add `git add -p`
- diff and options are present - "y,n,q,a,d,j,J,g,/,s,e,p,?" - option s
- Stage this hunk - option 1 of 2 if 2 hunks are discovered
- autodiscovered hunks have unchanged lines between them
- you choose hunk for hunk whether to stage or not
- now is the time to edit a hunk into different pieces
- now your are into manual hunk edit mode with the diff marks
- to remove - lines make them " ", to remove + lines delete them
- after ready you save your file and git stage it