# 85 Apply formatted patches

- Extracts author, commit message, and changes from a mailbox message and commits them to the current branch
- makes new commits
- similar to cherry-picking: same changes, different SHAs
- `git am feature/0001-some-name.patch` - am here is apply mailbox
- `git am feature/*.patch` - apply all patches from a directory
- `git am ../recent_comits/*.patch`
- the SHA are different but the content is the same
- if you only want to share the sum of all your changes then a diff patch may work best for you
- if you want to preserver the commit history then formatted patches are a better choice