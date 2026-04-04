# 32 Ancestry

- [ ] ^ - indicates the prior commit, or also called the commit that precedes it or also parent commit
- [ ] ~n = NTH PRIOR COMMIT if you leave just ~ it defaults to one so just the previous commit
- [ ] if you reference `abc123^` you reference the commit that preceed it
- [ ] you can also reference Grandparent commit using `abc123^^` double carret symbol
- [ ] a designation of `de14621f~2` is possible and means exactly the same as `abc123^^` or if you use `HEAD~2`
- [ ] example: `git log --oneline HEAD~6..HEAD^^`
- [ ] example: `git diff --stat HEAD~6..HEAD^^  `  
- [ ] you can use it with `` git show / log / diff` ``  and more