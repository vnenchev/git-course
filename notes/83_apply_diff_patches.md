# 83 Apply diff patches

- Apply changes in a diff patch file to the working directory
- make changes but not commits
- no commit history tranferred
- diff patches can be changes that have never been comitted at all
- `git apply output.diff`
- Lynda's repository view:
    - `pwd`
    - `git fetch`
    - `git log --oneline --graph --decorate --all`
    - `git apply output.diff` , here it is possible to have conflicts
    - `git status` - changes are in our working directory