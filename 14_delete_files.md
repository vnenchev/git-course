# 14 Delete files
- if you delete untracked file it will simply disappear from git tracking because no information for them yet
- first add the file to be tracked, and after that delete it if necessary
- there are 2 techniques to delete files, first is to delete the files manually 
- more laborious go to folder and manually delete with `rm <filename>` 
- second way is the git command for this `git rm delete_me.txt` - file is gone, and the changes are staged automatically but still commit is needed
- IMPORTANT USE CASE: to remove file from tracking but keep it locally use `git rm --cached <filename>` interestingly it doesn't accept `--staged`
- to remove all files from the repo but keep the commit history `git rm -r --cached .` afterwards just commit and you have empty repo but history is still present