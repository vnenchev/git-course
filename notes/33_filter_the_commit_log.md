33 # Filter the commit log

- git log can be used with filtering
- `git log --stat --oneline index.html` example
- `git log` show all commits, `git log file.txt` show logs for file.txt, `git log stylesheets/` only logs for this directory
- check commits `git show -s --oneline abc123` the shortest possible version of show
- `git log file.txt` or `git log stylesheets/`
- checkout the `git help log` for more information, a lot of filtering methods available
- `git log -n 3` limit the results to three commits
- or also `git log <SHA>..<SHA>` you will see the commit after the first mentioned and including the second/more recent commit/
- filter commits by date
    - `git log --since=2024-06-02`
    - `git log --until="3 days ago"`
    - `git log --after=2.weeks --before=3.days`
- filter by author
    - `git log --author="Name Surename"`
- using Regular expressions
    - `git log --grep="bug"` => this is the very basic usage of regex
    - to use the FULL FUNCTIONALITY OF REGEX use `git log -E --grep="b.+g"`
- and filters can be combined `git log --author="Name" -n 3 index.html`