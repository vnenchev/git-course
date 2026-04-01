# 25 Remove untracked files

- sometimes files no longer needed, temporary files, output files, compiled code, operating system artifacts, environment files or just files that we don't want to track and delete them
- `git clean` remove files for good so be careful, it doesn't work without any options -n is for dry run
- `git clean -n` will do dry run and just prompt you what will be removed
- `git clean -f` this is force clean files and actually removes untracked files
- if file is already staged `clean -f` won't remove it
- if staged `git restore --staged <filename> / git clean -n / git clean -f` , old alternative `git checkout HEAD <filename>`, `git clean -n`, `git clean -f`
- be sure if you need the files because they are deleted for good and not recoverable
- you can use also `git clean -i` for interactive mode, there you can pick manually files or use excluding pattern for more complex selections
- if you use `git clean -fd` - it will remove the untracked directories and the files inside, `-d` removes untracked directories even if empty recursively