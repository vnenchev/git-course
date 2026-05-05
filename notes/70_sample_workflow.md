# 70 Sample workflow 

- Kevin workspace:
    
    - `git switch main` make sure you are on your main branch
    - `git fetch` the first thing to do is to fetch any possible changes - there are some commits go and get them
    - `git merge origin/main` merge your remote tracking branch with your local branch to be in sync
    - create a new branch for product review page and switch to it `git switch -c product review`
    - product page is now ready so `git add product_review.html`
    - `git commit -m "Add product review form"` - at this stage all changes are local
    - not ready to merge the changes yet because Lynda needs to see it first
    - `git fetch` again let's see if there are other commits in the mean time
    - `git push -u origin product_review` - push to branch for others to see it
    - at this point an email is sent to collaborators to see the future and assess
- Lynda workspace:
    
    - `git fetch` see for changes, notices product_review
    - `git branch product_review origin/product_review` creates new branch from the source origin/product_review
    - `git switch product_review` Lynda switches to the new branch to check the changes
    - `git log` lets see the commits
    - `git show 832jk23k` what is changed
    - she decides to improve the form by adding star review option
    - she makes that change and `git commit -am "Add stars UI to product review"`
    - the changes are now in the local repository but she needs to upload them
    - `git fetch` she fetches again to be sure
    - she uses `git push` to send the changes to the remote
    - Lynda sends an email to explain what has she done
    - she can switch back to the work she has been doing
- Kevin workspace part 2
    
    - `git fetch` again to see for any change
    - don't use `git pull` right away because want to review the changes before that
    - `git log -p HEAD..origin/product_review` - with this you can see the difference between the old state and the work she has done
    - at the moment Kevin agrees it is a nice improvement and want to merge the changes
    - merge into local product review `git merge origin/product_review`
    - let's merge into the main branch of Big Collectibles as there is permission to do it
    - `git switch main`
    - `git pull` => it is fetch + merge, this is for others commits
    - `git merge product_review` - this is your feature
    - `git fetch` before doing git push, optional to be sure that no new commits on the main branch