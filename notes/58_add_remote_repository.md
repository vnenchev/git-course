# 58 Add remote repository

- if you haven't created your repo the fastest way to start is to create your repository on Github and do a `git clone`
- if you have already code locally you don't have a choice than to setup a remote and push it
- `git remote add origin https://github.com/techprepared/big_star.git`
    - `git remote -v` => remote verbose shows more information
    - `cat .git/config` shows you more detailed information about your remote
    - to remove remote use `git remote rm origin`
- `git branch -M main` this is forcefully renaming of your primary branch to main for compatibility
- `git push -u origin main`
- to remove remote you can type `git remote rm origin`