# git-command
Git command list for beginner 

### Install the git

```
    - git --version
    - git config --global user.name "name"
    - git config --global user.email "youremail@yourdomain.com""
```


### create project & add project member with permission & commands

```
add ssh key to gitlab
    - ssh-keygen -t rsa -b 4096 -C "youremail@yourdomain.com"
clone repo
    - git clone repo {foldername}
create branch
    - git branch {branchName}
delete branch
    - git branch -d {branchName}
create a file
    - touch {fileName}
git status
    - view the changes files
add files
    - git add {fileName or . for all}
reset added files
    - git reset {fileName} -m
git diff
    - git diff {fileName} #+ is new changes/ - is old changes
discard file changes
    - git checkout {fileName}
git stash
    - git stash
    - git stash list
    - git stash apply -{id}
git commit to that branch
    - git commit -m {comment}
push to server a merge request
    - git push origin {branchName}
merge the code
    - git merge {SourceBranch} {DestinationBranch} #code level one way
    - git pull origin {DestinationBranch} # code level second way
    - go to server and merge the request #by gitlab gui
conflict resolve
    - by manual find the diff and necessary
git log
    - git log
list branch
    - git branch
switch branch
    - git checkout {branchName}
revert the merged request
    - git revert {commitID}
    - go to server and revert the merge one by one #by gitlab gui
inspect the code
    - git log -L Start,+need:{fileName}
purpose of gitignore
    - this is omit the unwanted file from local to server. Ex: log or vendor file no need to push to server
existing folder
    - git init
    - git remote add origin {repo}
    - git push origin {branch}
    - git error: `fatal: refusing to merge unrelated histories`  Solution : add command `--allow-unrelated-histories`

```
