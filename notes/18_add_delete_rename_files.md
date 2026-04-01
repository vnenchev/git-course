# 18 Add, delete and rename files
- untracked files are not added by using `git commit -a` because you need to make your files tracked before that, you should use `git add .` and after that `git commit -m 'message'`
- if you just drop a file into your project it will be shown as untracked
- when you use `git add .` you add both tracked and untracked files
- to add only the tracked file use `git add -u`
- if the file is already tracked you can use shortcut `git commit -am 'your message here'`
- rename file with `git mv humans.txt README.md`
- remove file with `git rm images/big-hero-extra-large.jpg`
- in all cases use the git version of the commands and not pure OS commands when possible
- delete UNTRACKED directories `git clean -n -d` to discover what will be deleted, `git clean -f -d` delete the directories even if nonempty