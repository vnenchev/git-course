# 57 Configure Github credentials

- one way is to generate Access tokens, it is a part of two way authentication which is mandatory since 2021
    - enter this token instead of password
- store token to send automatically - this is what is show by the author
    - https://docs.github.com/en/get-started/git-basics/caching-your-github-credentials-in-git
    - search for windows installation of github cli
    - on CMD type `gh auth login` and follow instructions
    - choose: Github => HTTPS => y => login with your browser
- SSH keys
    - documentation for setting tokens is available at https://docs.github.com
- search for credentials => "Caching your Github credentials with Git"
- procedure to follow:
    - `gh auth login`
    - Github.com
    - HTTPS
    - Yes
    - Login with a web browser
    - Copy your one time code and authenticate