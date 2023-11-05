# The popular Git commands

This document will show these git commands usual use in the fact

## Configure for git in the first time

|      | Git command                                 | Description               |
| ---- | ------------------------------------------- | ------------------------- |
|      | git config --global user.name "Your name"   | Set name displayed in git |
|      | git config --global user.email "Your email" | setup your account        |
|      | git config --list                           | See configuration         |
|      | cat ~/.gitconfig                            | See all configuration     |

## General command

|      | Git command                                            | Description                               |
| ---- | ------------------------------------------------------ | ----------------------------------------- |
|      | git init                                               | Initial new project                       |
|      | git remote add "remote repository name" [git_repo_URL] | Link local and remote repository          |
|      | git status                                             | check status                              |
|      | git clone [git_repo_URL]                               | down project from remote repo             |
|      | git fetch                                              | check latest change on remote repo        |
|      | git pull                                               | Pull all change from remote to local repo |

## Branch and switching 

| **Id** | Git command                     | Description                               |
| ------ | ------------------------------- | ----------------------------------------- |
| 1      | `git checkout "Branch Name"`    | change branch which u want                |
| 2      | `git checkout -b "branch name"` | Create and switch into that branch        |
| 3      | `git branch`                    | Check current branch which we're standing |
| 4      | `git branch -D "branch name"`   | To del indicated branch                   |

## Commit

| **Id** | Git command                    | Description                                                  |
| ------ | ------------------------------ | ------------------------------------------------------------ |
|        | git add [file name]            | Add indicated file from working directory to local repository |
|        | git add .                      | Add all changed file from WD to Local Repository             |
|        | git reset [file name]          | Remove indicated file out of local repository                |
|        | git reset --sort  `commitID`   | fall back indicated commit (all change in after indicated commit will be move in stage area) |
|        | git reset -- mixed `commitID`  | fall back indicated commit (all change in after indicated commit will be move working directory) |
|        | git reset --hard `commitID`    | fall back indicated commit (all change in after indicated commit will be deleted) |
|        | git commit -m"comment"         | snapshot changing in WD                                      |
|        | git commit --amend -m"Comment" | Edit commit in WD                                            |
|        | git push origin branch-name    | Push commit from local up remote                             |
|        | git log -n                     | Watch commit history (n: line)                               |
|        | git log --oneline              | watch commit history                                         |
|        | git log --graph --oneline      | watch commit history clearly                                 |
|        | git diff                       | watch these change between WD and LC repo                    |
|        | git diff -> a.patch            | save these change between WD and LC repo to file a.patch     |
|        | git show                       | show these news in commit                                    |

## Merge and Rebase

| Command                         | Description                                                  |
| ------------------------------- | ------------------------------------------------------------ |
| git merge `feature branch name` | Merge indicated branch into **current branch have being checkouted** |
| git rebase `main`               | Checkout from the latest commit of main branch (Must be standing in the branch which u you to checkout) |

## Resolve conflict

* Using Rebase:

| ID   | Step to resolve                       | Description                                                  |
| ---- | ------------------------------------- | ------------------------------------------------------------ |
| 1    | `Checkout "Feature branch"`           | Make sure u have been checkout the branch you want to rebase |
| 2    | `git rebase -i master`                | This command with meaning checkout from latest commit of **branch master** |
| 3    | resolve conflict                      | Watch in code where make conflict and fix it                 |
| 4    | `git push origin "feature branch" -f` | flag `-f` with mean that the new commit just pushed will overwrite the previous commit on the feature branch |

* Using Merge: (In process and may be update in the future)

| ID   | Step to resolve | Description |
| ---- | --------------- | ----------- |
| 1    |                 |             |

<h2 align="right">
   	Thai Tran
</h2>
