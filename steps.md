# Setup:

## go to working folder:

% cd "PWD"

## write readme:

echo "# PWD" >> README.md

git init

Initialized empty Git repository in PWD/.git/
% git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        nameX.txt
        README.md

## Stage your changes:

git add .
% git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   nameX.txt
        new file:   README.md






# Initiate to Main

% cd PWD

## Initialize a new Git repository:

% git init
Reinitialized existing Git repository in PWD/.git/

## To verify what branch you are in:

% git status

On branch main
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean

## List all remote branches:

% git branch -r
  origin/main
  origin/temp


## List both local and remote branches:

% git branch -a
* main
  remotes/origin/main
  remotes/origin/temp

## To verify your current branch and status:

% git status

## To pull and switch to a specific remote branch:

% git checkout -b temp origin/temp
branch 'temp' set up to track 'origin/temp'.
Switched to a new branch 'temp'

## First commit

% git commit -m "first commit"

## fix wrong credentials:

% git config --global user.email "XXXXXXX+USERNAME@users.noreply.github.com"

on https://github.com/settings/emails > Keep my email addresses private > We’ll remove your public profile email and use...

% git commit --amend --reset-author --no-edit


# Switch to the main branch
git checkout main

# Pull the latest changes
git pull origin main

# Merge the temp branch into main
git merge temp

# Push the updated main branch to GitHub
git push origin main
