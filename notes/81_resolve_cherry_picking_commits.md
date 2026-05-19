# 81 Resolving cherry picking commits

- your cherry picked commits may have conflicts that need to be resolved
- `git cherry-pick 3k23jlk3` - commit which will create conflict
- After resolving the conflicts, mark them with
- `git add/rm <pathspec>` then run
- `git cherry-pick --continue`.
- You can instead skip this commit with `git cherry-pick --skip`.
- To abort and get back to the state before `git cherry-pick`,
- run `git cherry-pick --abort`.
- Disable this message with `git config advice.mergeConflict false`
- the conflict place is marked as with merge with `<<< and >>` signs so look for them
- after edits add your file with `git add index.html` and check with `git status`
- now you are ready to continue with `git cherry-pick --continue`