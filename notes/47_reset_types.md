# 47 Reset types

- resets the branch to when a specified commit was made
- moves branch and HEAD pointer to a specific commit
- new commits will begin at HEAD pointer
- former descendants commits will be orphaned unless another branch or tag references them
- use caution if commits were already shared, you may have different history than your collaborators
- you have soft reset, mixed reset, hard reset
- all move the branch and HEAD pointer
- change staging tree and working directory differently