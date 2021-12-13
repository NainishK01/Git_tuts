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
