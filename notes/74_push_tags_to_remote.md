# 74 Push tags to remote

- the tags created to the moment are local tags, tags are local unless shared to a remote
- `git push` does not transfer tags by default
- this is good because you can create tags locally and not spam everyone else
- if you want to share tags it must be done explicitly
- once transferred, collaborators may use `git fetch` to automatically retrieve shared tags
- you can push a single tag with `git push origin v1.0` a branch and a tag are just references to a SHA
- push all of your tags `git push origin --tags`
- you can delete remote tag `git push -d origin v1.0`
- branch and tags are next to each other in GitHub
- let us push our tags to the remote, first list them `git tag -l`
- `git push origin v1.0`
- `git push --tags` here we don't specify origin because it is assumed
- if it was by mistake `git push -d origin v1.0`
- now we are switched to the Lynda's repository to see her view
- she issues `git tag -l` and there are no tags
- if she does with `git fetch` the tags will be also fetched