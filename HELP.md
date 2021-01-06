# Git Commands
## Version
```
git --version
```
## Help
```
git help
```
## Configurate Global User Name and Email
```
git config --global user.name "John Doe"
git config --global user.email "john.doe@example.com"
```
## Edit All Global Configuration
```
git config --global -e
```
## List All Global Configuration
```
git config --global -l
```
# Init Repository
```
git init
```
# Repository Status
```
git status
```
# Simplify Repository Status
```
git status -sb
```
# Add All Files
```
git add .
```
# Add Modified Files
```
git add -A
```
# Add Files
```
git add <file>
```
# Unstage Added Files
```
git reset <file>
```
# Commit
```
git commit -m "The commit message."
```
# Reverse All Changes
```
git checkout -- .
```
# Reverse File Changes 
```
git checkout -- <file>
```
# Log
```
git log
```
# Log in One Line
```
git log --oneline
```
# Log With All Detail
```
git log --oneline --decorate --all --graph
```
# Create an Command Alias
```
git config --global alias.alias-name "git-command option-1 option-2 option-n"
```
* ## Examples
    ```
    git config --global alias.lg "log --oneline --decorate --all --graph"
    ```
    ```
    git config --global alias.sb "status -sb"
    ```