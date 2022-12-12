# Git tips

- Basics

  - `git init` = initialise a git repo
  - `git clone <url>` = clone the repo @ URL into current directory
  - `git remote --list` = list all remote urls

  - to remove a Git repo just find the hidden `.git` folder and delete it

- Git branch

  - `git checkout -b <name>` = make a new branch and checkout into it
  - `git branch --list [branch regex]` = list all branchs or list branches matching regex
  - `git switch <branch name>` = switch to branch, kind of replaces `checkout` in the sense it does the same as `git checkout <branch name>`. The devs of git apparently added `switch` command to make a distinct command rather than
    `checkout` swiss army knife approach.
  - `git merge <branch name>` = merge the named branch into the current checkedout branch
  - `git branch -d <branch name>` = delete branch name
    - `-d` = delete

- Naming convention tips

  - `wip` `test` `feat` = use grouping tokens - may use slash to help group like branchs ex. `wip/foo` `test/bar`

- General

  - `git stash` = stash away your changes on that branch so you can save them without them following you to another branch. Must be staged!
  - `git stash pop` = un-stash those changes you stashed earlier
  - `git stash list` = show saved stashes
  - `git stash save "add a info msg to stash"` = add a informative message to your stash

- Dangerzone
  - `git rm -r --cached` = removes all files from tracking (if .gitignore not ignoring, may be as it won't ignore a previously tracked file)
    - `-r` recursively complete command from current location down through folder heirarchy
    - `--cached`
  - `git rm --cached <filename>` = remove file from staging
  - `git reset` = resets the staging area
