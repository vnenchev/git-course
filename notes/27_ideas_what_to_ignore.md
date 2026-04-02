# 27 Ideas what to ignore

- operating system-generated files
- log files, execution logs
- compiled source code / build artifacts
- databases are commonly excluded
- credentials and other secrets / libraries and plug-ins
- assets ( images, pdf's, videos), generally static files
- compressed files `\*.zip` not expected to be changed
- a collection of useful .gitignore templates -> [ignore templates on Github](https://github.com/github/gitignore)
- if the file is tracked `git rm --cached <path to file>` -> add rule to your .gitgnore and make a commit for it