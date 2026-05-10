# Git:
Version control system that allows to make changes and track them

# GitHub:
Website that allows to make changes using git

## Configuring git:
+ username: git config --global user.name "My-Name"
+ user email: git config --global user.email "someone@gmail.com"
+ check credentials: git config --list

## Other commands:
+ clone: git clone "Prefer HTTPS link"
+ status: git status
+ add: git add file.name (to stage)
+ restore: git restore --staged file.name (to unstage)
+ commit: git commit -m "commit message"
+ push: git push origin main
+ pull: git pull origin main

## Starting with local repo:
+ init: git init
+ origin add: git remote add origin repo.link
+ verify remote: git remote -v
+ to check branch: git branch
+ rename branch: git branch -M main
+ pushing with upstream: git push -u origin main

## Branch commands:
+ change branch: git checkout branch.name
+ create new branch: git checkout -b newbranch.name
+ delete branch: git branch -d branch.name (to should be on some other branch to delete this branch)

### (Note: when new branch say 'feature1' is created then pushing command should be performed standing on this branch itself something like : git push origin feature1)

## Merge code:
### way1: 
+ to see diff: git diff branch.name (this says the difference between the branch present and the branch.name given) 
+ git merge branch.name (then select whatever the changes your prefer)

### way2:
+ Through PR

## Undoing changes:
+ staged changes: git reset file.name (or) git reset
+ commited changes (for 1 commit): git reset HEAD~1
+ commited changes (for many commits): git reset commit.hash (or) git reset --hard commit.hash
+ check all commits: git log

## Fork:
