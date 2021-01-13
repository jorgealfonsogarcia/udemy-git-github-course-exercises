# Git Commands
## Version
```sh
git --version
```
## Help
```sh
git help
```
## Configurate Global User Name and Email
```sh
git config --global user.name "John Doe"
git config --global user.email "john.doe@example.com"
```
## Edit All Global Configuration
```sh
git config --global -e
```
## List All Global Configuration
```sh
git config --global -l
```
## Init Repository
```sh
git init
```
## Repository Status
```sh
git status
```
## Simplify Repository Status
```sh
git status -sb
```
## Add All Files
```sh
git add .
```
## Add All Modified Files
```sh
git add -A
```
## Add Files
```sh
git add <file>
```
## Unstage Added Files
```sh
git reset <file>
```
## Commit
```sh
git commit -m "The commit message."
```
## Add All Modified Files and Commit
```sh
git commit -am "The commit message."
```
## Amend Last Commit Message
```sh
git commit --amend -m "The new commit message."
```
## Reverse All Changes
```sh
git checkout -- .
```
## Reverse File Changes 
```sh
git checkout -- <file>
```
## Log
```sh
git log
```
## Log in One Line
```sh
git log --oneline
```
## Log With All Detail
```sh
git log --oneline --decorate --all --graph
```
## Create an Command Alias
```sh
git config --global alias.alias-name "git-command option-1 option-2 option-n"
```
* ### Examples
    ```sh
    git config --global alias.lg "log --oneline --decorate --all --graph"
    ```
    ```sh
    git config --global alias.sb "status -sb"
    ```
## Get the Difference Between the Current Files Unstaged and the Last Commit
```sh
git diff
```
## Get the Difference Between the Staged Files and the Last Commit
```sh
git diff --staged
```
## Reset Soft Last Commit
```sh
git reset --soft HEAD^
```
## Reset to an Specific Commit (Don't Delete the Modified Files)
```sh
git reset --mixed <COMMIT-HASH>
```
* ### Example
    ```sh
    git reset --mixed 63c9c99
    ```
## Reset to an Specific Commit (Delete the Modified Files)
```sh
git reset --hard <COMMIT-HASH>
```
* ### Example
    ```sh
    git reset --hard 63c9c99
    ```
## Reference Log (Shows All Repository History)
```sh
git reflog
```
## Change File Name
```sh
git mv <old-filename> <new-filename>
```
* ### Example
    ```sh
    git mv demo-04-heroes/destroy-world.txt demo-04-heroes/save-world.txt
    ```
## Delete File
```sh
git rm <file>
```
* ### Example
    ```sh
    git rm demo-04-heroes/save-world.txt
    ```
## Update Renamed (Or Deleted) Files When It's Applied Outside Git
```sh
git add -u
git add -A
```
## Create a New Branch
```sh
git branch <new-branch-name>
```
* ### Example
    ```sh
    git branch my-new-branch
    ```
## Change Branch
```sh
git checkout <branch-name>
```
* ### Example
    ```sh
    git checkout my-new-branch
    ```
## List Branches
```sh
git branch
```
## Get the Difference Between Branches
```sh
git diff <branch-1-name> <branch-2-name>
```
* ### Example
    ```sh
    git diff my-new-branch master
    ```
## Merge a Branch into the Current Branch
```sh
git merge <branch-name>
```
* ### Example
    ```sh
    git merge my-new-branch
    ```
## Delete a Branch
```sh
git branch -d <branch-name>
```
* ### Example
    ```sh
    git branch -d my-new-branch
    ```
## Create and Change to a New Branch
```sh
git checkout -b <new-branch-name>
```
* ### Example
    ```sh
    git checkout -b my-new-branch
    ```
## Create a Tag to the Current Commit
```sh
git tag <tag-name>
```
* ### Example
    ```sh
    git tag v1.0.0
    ```
## List Tags
```sh
git tag
```
## Delete a Tag
```sh
git tag -d <tag-name>
```
* ### Example
    ```sh
    git tag -d v1.0.0
    ```
## Create an Annotated Tag to the Current Commit
```sh
git tag -a <tag-name> -m "Message"
```
* ### Example
    ```sh
    git tag -a 1.0.0 -m "Version 1.0.0"
    ```
## Create an Annotated Tag to a Specific Commit
```sh
git tag -a <tag-name> <COMMIT-HASH> -m "Message"
```
* ### Example
    ```sh
    git tag -a 0.1.0 1989054 -m "Alpha Version."
    ```
## Show Tag Info
```sh
git show <tag-name>
```
* ### Example
    ```sh
    git show 0.1.0
    ```
## Stash
```sh
git stash
```
## Stash with a Message
```sh
git stash save "<message>"
```
* ### Example
    ```sh
    git stash save "Adding new README.md file."
    ```
## List the Stash
```sh
git stash list
```
## List the Stash with the State
```sh
git stash list --state
```
## Recover the Stash
```sh
git stash pop
```
## Drop the Stash
```sh
git stash drop
```
## Drop a Specific Stash
```sh
git stash drop <stash-id>
```
* ### Example
    ```sh
    git stash drop stash@{1}
    ```
## Clear All the Stash
```sh
git stash clear
```
## Apply a Specific Stash
```sh
git stash apply <stash-id>
```
* ### Example
    ```sh
    git stash apply stash@{1}
    ```
## Stash Keeping Index
```sh
git stash save --keep-index
```
## Stash Including Untracked
```sh
git stash save --include-untracked
```
## Show the Stash
```sh
git show stash <stash-id>
```
* ### Example
    ```sh
    git show stash stash@{1}
    ```
## Show the Stash
```sh
git rebase <branch-name>
```
* ### Example
    ```sh
    git rebase master
    ```
