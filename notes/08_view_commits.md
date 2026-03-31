# 8 View commits
- `git log` list of commits in reverse chronological order, most recent commit at the top if you want the opposite `git log --reverse`
- you can track individual file changes `git log index.html` or try `git log --follow index.html`
- there is `SHA` number, author, date, commit message, it looks something like `commit 60bee641e189d84feed28e5e4039050b16a9cd4f`
- `git show <here you copy the SHA number of the looked commit>`
- now it is very important that additionally to other information now you see what is inside of the commit and changes are pointed
- if your `diff` is showing `--- /dev/null` then the file was not existing before
- use `git status / git add / git commit / git log / git show`
- log page has a ton of options, you need to spend some time trying some variants `git help log`
- if we want to view the content of a commit we better use `git show <SHA>` command, git show is also very broad so take your time