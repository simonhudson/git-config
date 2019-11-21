# Git config
Useful git config/alias stuff

## Alias
### Checkout
* Set -> `git config --global alias.co '!f() { git checkout "$1"; }; f'`
* Use -> `git co my-branch`

### Create new branch
* Set -> `git config --global alias.nb '!f() { git checkout -b "$1"; }; f'`
* Use -> `git nb new-branch`

### Push new branch
* Set -> `git config --global alias.pnb '!f() { git push -u origin "$1"; }; f'`
* Use -> `git pnb new-branch`

### Delete local branch
* Set -> `git config --global alias.dl '!f() { git branch -D "$1"; }; f'`
* Use -> `git dl my-branch`

### Delete remote branch
* Set -> `git config --global alias.dr '!f() { git push origin --delete "$1"; }; f'`
* Use -> `git dr my-branch`

### Log commits from today
* Set -> `git config --global alias.donetoday 'log --since="00:00:00" --no-merges --oneline --author=<you@email.com>'`
* Use -> `git donetoday`
