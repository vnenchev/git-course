# Working with a remote

- origin/main is a reference to a copy of whatever the remote has in its main branch
- no live connection is kept, only updates the remote references from time to time, is it works even without network
- main is a reference to the local main branch
  - we need to periodically perform fetch to see what's on the remote
  - REMEMBER with git fetch you update your origin/branch and if you want the remote changes in your local working branch you NEED to git merge
- of course shortcut for both operations is git pull but sometimes you are in the middle of something and don't want to merge immediately