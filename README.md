### Configure username and email
```
  git config --global user.name <name>
  git config --global user.email <email>
```
### Initialize empty git repo
```
  git init
```
### To check status and if it is a part of repo
```
git status
```
### Add files to staging environment (files ready to commit)
###### Stages all changes
```
git add --all[-A]
```
###### Stages new files and modifications, without deletions
```
git add .
```
###### Add specific files
```
git add <filename>
```
### Commit the staging environment
```
git commit -m "<message>"
```
### To view history of commits
```
git log
```
### For help
```
git help --all
git <command> -help
```
### To branch new/seperate version
```
git branch <branch-name>
```
### To move to new branch from "master" branch, or switch back to master
```
git checkout <branch-name/master>
```
### To checkout previous commit, use 'git log' to get the hash or particular commit and use
```
git checkout <hash>
```
### If we're on the branch and want to fix some issue from master without disturbing either master or branch, we can create emergency branch and later merge
```
git checkout -b <emergency-branch-name>
```
### To merge branch such as emergency-branch to master, first switch to master then merge
```
git checkout master
git merge <branch-name>
```
Or,
```
git merge <branch-name> master
```
### To delete branch
```
git branch -d <branch-name>
```
## Push local repo to github
###### Create remote connection
```
git remote add origin <url>
```
###### Push to remote conn on master branch
```
git push -u origin master
```
## Difference between 'merge' and 'rebase'
Both 'merge' and 'rebase' are used to integrate changes from one branch to another, but with different way.
'Merge' keeps the history of commits of both branches. While 'Rebase' re-writes the project history by creating brand new commits for each commit in the original branch.
In other words, rebase gives cleaner project history, but if you want to track every single commit change merge is useful.
