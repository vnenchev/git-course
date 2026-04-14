# 50 Hard reset

Moves branch and HEAD pointer
- changes staging index to match repository
changes working directory to match repository - - therefore you see nothing to commit, working dir is clean
- change the repository state and discard all changes
- useful to permanently undo commits
- be careful not to lose any useful changes
only if you do commits after that the ability to go - back to those commits is lost
be careful to reset commits that are shared with - other people
- interesting ability to use old branch to catch up with new one using `git reset --hard main` here we catch up with main moving upwards
any changes on old branch that were different are - gone
interesting case is that you can use git reset hard - not only to go back in time but also go forward
- use this a lot with a staging branch where i want to stage changes for a client to look exactly as different branch