# 76 Interactive commands

- update command will add working tree state to the staged set of changes
- revert command reverd staged set of changes back to the HEAD version
- add untracked add contents of untracked files to the staged set of changes
- diff command will show us diff between HEAD and index, its like `git diff --staged` and `git diff -cached`
- we have two modified files => about and cart html
- update option is similar to `git add <filename>` from command line, now type `git add -i`
- here you have option to select file by number, \* - means that file is selected for staging
- if you just press enter the prompt says What now> for you to select what happens next
- revert option works the same way, you mark files by their numbers and watch for the \* designator
- if you have untracked file you need to use option 4 add untracked => same nav as update and revert
- option 7 diff gives you difference but only for the staged files
