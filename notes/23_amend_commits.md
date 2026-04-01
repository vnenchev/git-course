# 23 Amend commits

- git allows the most recent commit to be amended, used for immediate adjustments
- can edit set of changes and/or commit message
- prior commits can only be changed with advanced techniques (rebase, reset)
- `git commit --amend` and if you have changes stored in the staging area they will also be applied VERY IMPORTANT SO STAGE THEM IF YOU WANT THEM INCLUDED
- you can also see the changes file wise with `git show --stat`
- `git commit --amend` doesn't make a new commit but changes the SHA of the last commit
- beware that if you've already pushed the commit to a remote, amending rewrites history so you'll need to force push `git push --force-with-lease`
- `--force-with-lease` preventing you from accidentally overwriting their work
- when you amend a commit you change its SHA