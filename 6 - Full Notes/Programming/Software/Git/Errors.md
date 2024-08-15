
Tags: [[Fixes]]

----------------------------------------
### Error

- "Please make sure you have the correct access rights and the repository exists"

### Fix

- run: `git remote set-url origin git@github.com:username/repository.git`

[Stackoverflow link](https://stackoverflow.com/questions/25927914/git-error-please-make-sure-you-have-the-correct-access-rights-and-the-reposito)

----------------------------------------

### Error

- "fatal: The upstream branch of your current branch does not match"

### Fix

- run: `git branch --unset-upstream`
- run: `git push --set-upstream origin main`

---------------------

### Error

- Permission denied

### Fix

** Generate a token -> github settings -> developer settings -> personal access token

- run: `git remote set-url origin https://<token>@github.com/<username>/<repo>`

[Stackoverflow link](https://stackoverflow.com/questions/71953666/remote-permission-to-repository-denied-url-returned-error-403)
