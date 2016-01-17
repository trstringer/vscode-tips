# Version Control (Git)

## Create/Initialize the repository

1. Switch to the Git workbench view (`CTRL+SHIFT+G`)
2. Select *initialize repository*

## Commit changes

1. Switch to the Git workbench
2. Do one of the following (depending on if you want to commit all or select changes):
 - to **commit all changed files**, type in a commit message and hit `CTRL+ENTER`
 - to **commit only select changes**, click the `+` icon to stage those files, type in a commit message and then hit `CTRL+ENTER`
 
## Branches

#### Create a new branch (command palette)

`git branch <new-branch-name>`

#### Checkout a branch (command palette)

`git checkout <branch-name>`

#### Publish local branch to remote repository (command palette)

`>Git: Publish`

## Synchronize changes between local and remote

> :bulb: When you "synchronize" in VS Code between a local and remote repository, this is just shorthand for two consecutive operations:

> 1. `git pull` from remote to local
> 2. `git push` from local to remote

#### Command palette

`>Git: Sync`

#### GUI

- In the status bar there is a button next to the branch name that, once clicked, will synchronize between the local and remote repo
 
## Show Git commands that are being executed

1. Open up the output window (`>View: Show Output` from the command palette)
2. Ensure that you are on the `Git` channel
3. Watch the git commands that VS Code is executing as you interact with the repository through the IDE