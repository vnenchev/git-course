# 28 Globally ignore files

- this is user level settings instead of individual project level settings which is `.gitignore`
- just need to tell git where is the global file `git config --global core.excludesFile ~/.gitignore_global`
- the above ignores for all projects for this user and global level is the default configuration
- the location of your global ignore file is completely configurable but check your `~/.config/.gitconfig`
- this settings are not shared with collaborators and are just for you to use
- if settings overlap then .gitignore on project level takes precedence or whichever file is last