# 2 Git installation
<!-- ![Where to download Git](../gifs/where_to_download_git.gif) -->
<div align="center"><img src="../gifs/where_to_download_git.gif" width=350 alt="where to download git">
<div>

- https://git-scm.com - go to download page, check the version for your os (x64, arm64, portable_thumbdrive edition)
- after installation you can check on cli what version do you use and if it is ok `git --version`
- if you want to make `git bash` your default terminal `"terminal.integrated.defaultProfile.windows": "Git Bash"` this line goes to `ctrl+shift+p` search for "User settings JSON", click on it and add the line
- next time when you open your VS Code your terminal will be Git Bash
- to update Git if newer version is release on Windows you need `git update-git-for-windows`, if installing by default autoinstaller shows only new options
- this is a good time to pick a place on your hard drive for storing your repositories
- many folks choose something like `user/Documents/projects`,`user/projects` or whatever you like, but the idea to keep everything organized will pay off long term
- and if you skipped the [history of Git and centralized vs distributed VCS](01_centralized_vs_distributed_vcs.md) and still interested
- lets go to the interesting stuff of [Git configuration](03_configuration.md)