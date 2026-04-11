# 43 Merge branches

- begin with clean branch with clean working directory
- switch to the receiving branch
- MERGE ALWAYS CREATE NEW COMMIT SO BE READY TO WRITE COMMIT MESSAGE
- `git log --graph --all --oneline --decorate`
- look for the split commit /called merge base/ and perform git merge-base seo_edits => you will find the split commit here
- `git diff <split commit>..<branch to merge>`
- git merge seo_edits performed from the receiving branch which is usually master
- merge commits usually have two parents
- git to tell us all the branches that have been fully merged git branch --merged to list is of merged branches, only fully merge
- show branches that haven't been merged git branch --no-merged