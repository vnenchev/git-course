# 59 Create a remote branch

- we need to add our shared branches manually, in this way we can have branches that are not shared as well as shared for collaboration
- `git remote show origin` if your remote is named origin you will see a lot of information
- remote origin / Fetch URL: https://github.com/techprepared/big_star.git / Push URL: https://github.com/techprepared/big_star.git / HEAD branch: (unknown)
- let us send the main branch to the remote repository
- `git branch -M main` is not necessary here because our main branch is called already main and here -M assures that your branch is named main and renames it to main if for example is called master according to previous versions of git
- Optionally delete old master on remote `git push origin --delete master`
- `git push -u origin main` - push the main branch to the origin remote, -u is helpful it just setup for the remote branch
- `git branch` is a command that shows only local branches
- `git branch -r` shows the remote branches
- `git branch -a` shows all branches local and remote
- now try again `git remote show origin`
- you can find this information in => `ls .git/refs/remotes/origin/main`