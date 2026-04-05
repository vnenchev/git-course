# 38 Switch branches with uncommited changes

- can switch when changes in working directory can be applied to branch version
- can switch when changes in working directory are untracked or ignored files
- if changes can be applied they persist in the working directory or staging even after the switch
- can't switch when changes in working directory conflict with branch version
- what you can do:
    - commit the changes to the current branch
    - remove the changes or restore the changed files
    - switch branches while also discarding the changes
    - stash the changes temporarily
- switch branch and discard changes => `git switch -f mynewbranch` switch to the branch and discard the changes
