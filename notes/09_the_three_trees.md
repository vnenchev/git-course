# 9 The three trees
- the concept of a tree structure is widely adopted in Computer Science
- 
- three directories  Working directory / Staging tree / Repository, you do your version control from bottom to top when creating or top to bottom when correcting things
- just know that if you put the same algorithm toward the same date the result will be the same hash value
- you have working directory / staging area / repository (possibly remote but not mandatory)
- even if you copy just the first symbols from SHA 7 or more, you can refer to this commit
- there is a command called `git write-tree` which is executed once a new tree object appears, the command executes whatever is in staging area and writes it to the Git object database
- after `git write-tree` see `git cat-file -p commit-SHA` for more information about the objects, command prints (-p means pretty print) the contents of any Git object given its SHA hash