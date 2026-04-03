# 29 Track empty directories

- if directory is empty it is not tracked, there are cases when you want to track the directory structure
- standard procedure is to add empty file like `.gitkeep` and it is dotted because we hide it
- when you initially add the file to the directory git sees only the directory but when you stage your changes .gitkeep is visible
- beware that if you put in your gitignore file `somedir/` the directory will not exist when your collaborators fork the project
- you need to create exclude rule for the `.gitkeep` or `!/somedir/.gitkeep`