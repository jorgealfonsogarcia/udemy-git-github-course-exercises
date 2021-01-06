# Git Commands
## Version
```bash
git --version
```
## Help
```bash
git help
```
## Configurate Global User Name and Email
```bash
git config --global user.name "John Doe"
git config --global user.email "john.doe@example.com"
```
## Edit All Global Configuration
```bash
git config --global -e
```
## List All Global Configuration
```bash
git config --global -l
```
## Init Repository
```bash
git init
```
## Repository Status
```bash
git status
```
## Simplify Repository Status
```bash
git status -sb
```
## Add All Files
```bash
git add .
```
## Add All Modified Files
```bash
git add -A
```
## Add Files
```bash
git add <file>
```
## Unstage Added Files
```bash
git reset <file>
```
## Commit
```bash
git commit -m "The commit message."
```
## Add All Modified Files and Commit
```bash
git commit -am "The commit message."
```
## Amend Last Commit Message
```bash
git commit --amend -m "The new commit message."
```
## Reverse All Changes
```bash
git checkout -- .
```
## Reverse File Changes 
```bash
git checkout -- <file>
```
## Log
```bash
git log
```
## Log in One Line
```bash
git log --oneline
```
## Log With All Detail
```bash
git log --oneline --decorate --all --graph
```
## Create an Command Alias
```bash
git config --global alias.alias-name "git-command option-1 option-2 option-n"
```
* ### Examples
    ```bash
    git config --global alias.lg "log --oneline --decorate --all --graph"
    ```
    ```bash
    git config --global alias.sb "status -sb"
    ```
## Get the Difference Between the Current Files Unstaged and the Last Commit
```bash
git diff
```
## Get the Difference Between the Staged Files and the Last Commit
```bash
git diff --staged
```
## Reset Soft Last Commit
```bash
git reset --soft HEAD^
```
## Reset to an Specific Commit (Don't Delete the Modified Files)
```bash
git reset --mixed <COMMIT-HASH>
```
* ### Example
    ```bash
    git reset --mixed 63c9c99
    ```
## Reset to an Specific Commit (Delete the Modified Files)
```bash
git reset --hard <COMMIT-HASH>
```
* ### Example
    ```bash
    git reset --hard 63c9c99
    ```
## Reference Log (Shows All Repository History)
```bash    
git reflog
```
## Change File Name
```bash    
git mv <old-filename> <new-filename>
```
* ### Example
    ```bash
    git mv demo-04-heroes/destroy-world.txt demo-04-heroes/save-world.txt
    ```
## Delete File
```bash    
git rm <file>
```
* ### Example
    ```bash
    git rm demo-04-heroes/save-world.txt
    ```
## Update Renamed (Or Deleted) Files When It's Applied Outside Git
```bash    
git add -u
git add -A
```
