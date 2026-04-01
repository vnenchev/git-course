# 17 Make and review edits
- make some edits to your files
- perform `git diff` to see how git see the changes
-  
- use VSCode search functionality, and after that `git diff`, the result is long if you compare paragraphs
- the drawback is that even if a single word in a long paragraph is changed you see the whole paragraph as changed and not the particular place
- use `git diff --word-diff` to see word differences in much more readable fashion
- use `git diff --word-diff=color` or `git diff --color-words` which is another shorthand and more convenient
- use the search functionality to make changes to multiple files simultaneously