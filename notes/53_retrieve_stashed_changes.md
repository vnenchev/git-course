# 53 Retrieve stashed changes

- Stack behavior - what we add last is on the top of the list and other entries go down the list
- pop an item off the top of the stack
- may have conflicts
- `git stash pop` if without number pops the last stash
- otherwise `git stash pop <stash>`
- `git stash apply` it applies the changes not delete them in the stash and by default the top element
- when you pop a stash you drop the reference to it
- git stash apply 0 apply the zeroth element, the item remains and could be applied to other branch