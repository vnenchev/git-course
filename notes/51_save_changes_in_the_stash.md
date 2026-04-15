# 51 Save changes in the stash

- stash works like a stack, the last things you push its on the top of the stack
- Separate area for temporarily storing changes
it is different area than working, index, or -repository
stash your changes before other git operations - -changing branches, merging, resetting, rebasing and more
- stashing will clean out your working directory
- it stores uncommitted changes to a new stash entry
- you can have many change sets in the stash at once
- resets the staging index and working directory to HEAD
- stashed changes can be viewed, applied, or deleted
- stash your current changes using git stash push
- provide a message to the stash entry with `git stash push -m` - VERY GOOD IDEA
push only things that are staged `git stash push ---staged`
put everything except the staged => `git stash ---keep-index`
- git show-branch stash alternative way to see what is in the stash and on which branch
- with `git stash branch modification_branch` you can create a branch from your stash