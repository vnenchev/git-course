# 61 Remote tracking branch

- to strategy to periodically merge changes is also important also for remotes
- remote tracking is not to confused with tracked and untracked files
- local branch follows a remote branch closely
- where to watch for new commits by default
- where to send your commits by default
- the branch being tracked is called upstream branch and this is the branch on github normally
- upstream branch and remote tracking ( local - origin/main/ branch ) are closely related but upstream is on the internet and remote tracking is local branch
- upstream is set for local branches:
    - when created from remote branches, like when we clone remote repo
    - when pushed to a remote if -u option is included for "upstream"
- git can be configured to set upstream on push by default
- `git config --global push.autoSetupRemote true` - if you want to auto track any branch that you push to, so good idea to set this up
- if you forget to set initially `git push -u origin <branch>` you can use `git branch -u origin/<branch> <branch>` - you say set upstream for origin/branch and use `<branch>` as a source and origin as target
- `git branch -u origin/tracking_test tracking_test`
- see more info in cat .git/config
- to unset upstream there is option `git branch --unset-upstream` research more with `git help branch`