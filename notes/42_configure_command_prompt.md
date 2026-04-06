# 42 Configure command prompt

- display current branch name in command prompt
- go to github.com/git/git , look for completion script called git-prompt.sh
- the execution of the script depends on the version of the shell you have => `echo $SHELL`
- can check if script exist => on git bash type `__git_ps1` and if you see current branch then already set
- online path is [script file](https://github.com/git/git/blob/master/contrib/completion/git-prompt.sh) copy raw file
- save it to ~/.git-prompt.sh
- next step is to load this script and it depends what shell do you use
- for bash:
  - `nano ~/.bashrc`
  - `source ~/git-prompt.bash`
  - `PS1='\WS(__git_ps1 " ($s)" > '`
  - PS one stands for prompt script
  - close your current prompt window and open new one to see the effect