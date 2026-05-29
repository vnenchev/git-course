# 89 Squash commits

- fold two or more commits into one, exactly as it sounds like
- squash: combine changesets, concatenate commit messages
- fixup: combine changesets, discard this message and keeps the prior one
- uses first author in the commit series if multiple authors are present
    - pick 4jk23j4kl32 Redesign
    - squash jkki324jh Change image sizes => squashes this commit with the commit above it
    - fixup 32kjkl23k bug fix to the redesign => squashes these changes into the commits in lines one and two
    - squash 32o4j32 Adjust styles => squashes these changes with the changes from the previous commits
    - at the end you will have one commit from all of the four commits in the list
    - squashing could be a good way to clean up commits, or you can cleanup commits you have already made, as long as you haven't shared them yet