# 5 Initialize repository
- first choose a place where you want to place your repository (create a folder) `mkdir <foldername>`
- after that switch to it and be ready to start working in this folder `cd foldername`
 `git init` - in the directory of your choice, only after that you can access git commands
- `.git` directory contains all the files for the VCS/SCM to work, if you delete it all of the tracking is gone, this is how to verify if the repo is created
- again you can use `find .` to list all files and folders to see clearly the structure if on Linux
- `config` file contains the project level configuration
- if you run `git init` in an initialized git repo it won't throw out your history or commits, it will reinitialize the repository
- if you delete `.git` folder you destroy all of the information about your repository stored locally
- copy your repository is very simple just put your path `git clone my_repo ../my_repo_copy`
- to create quick sample file use `echo "some random text" > pretty.file` output redirection
- there is also the concept of bare repository, its a repo that contains only Git history and metadata and no working files
- bare repositories are meant to be shared endpoints
- `git init --bare /repos/my_project.git`
- the rule of thumb is - you work in normal repositories, you share through bare repositories, you never commit directly into a bare repo, only push to it
- bare repository has everything in it but it doesn't need working directory as normal repository because none of the contributors edit files directly on the server
- it is just a place that everyone agrees to exchange files 