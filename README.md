<<<<<<< HEAD
#Git

// Check version

`$ git --version`

// Set/Check current user name and email

`$ git config --global user.name USERNAME`

`$ git config --global user.email EMAIL`

`$ git config user.name`

`$ git config user.email`


// Change current directory
`$ cd working_directory`

// Create local git repository
`$ git init`

// After editing files in current directory, check status to see which files have been changed
`$ git status`

// Add files to queue to be commited
`$ git add <file>`

// Commit changes
`$ git commit -m “comment on commit”`

// If this is a new repository, create a repository in remote server using GUI
// Then follow the instruction in GitHub: add then push to the master

`$ git remote add origin https://github.com/justsangsue/repository_name.git`

`$ git push -u origin master`

#Manage Changes
=======
# LearnGit
A repo to learn git

# Git

// Check version
$ git --version

// Set/Check current user name and email
$ git config --global user.name USERNAME
$ git config --global user.email EMAIL
 
$ git config user.name
$ git config user.email


// Change current directory
$ cd working_directory

// Create local git repository
$ git init

// After editing files in current directory, check status to see which files have been changed
$ git status

// Add files to queue to be commited
$ git add .

// Commit changes
$ git commit -m “comment on commit”

// If this is a new repository, create a repository in remote server using GUI
// Then follow the instruction in GitHub: add then push to the master
$ git remote add origin https://github.com/justsangsue/repository_name.git
$ git push -u origin master

# Manage Changes
>>>>>>> dev

Stage is a “beffer area” for changes. Changes is moved into stage when doing “git add”

When doing “git commit”, changes will be applied and changed files will be recorded in “repo”. “HEAD” pointer points to the latest commit by default.

Working directory — add —> Stage — commit —> Repo 

To redo changes in working directory 
<<<<<<< HEAD

`$ git checkout -- <filename>`

After this, changed files will be recovered.

To unstage a change (cancel “git add”)

`$ git reset HEAD <filename>`

Now file is still changed, if want to get previous file, use `git checkout -- <file>`.

To undo a commit:
`$ git reset --hard HEAD^`
=======
$ git checkout -- <filename>
After this, changed files will be recovered.

To unstage a change (cancel “git add”)
$ git reset HEAD <filename>
Now file is still changed, if want to get previous file, use “git checkout -- <file>”.

To undo a commit:
$ git reset --hard HEAD^
>>>>>>> dev
log will also be removed as HEAD pointer is moved.
“HEAD^” means last version. 
“HEAD^^” means second last version. 
“HEAD-100” means 100th last version.
To put HEAD pointer back to a specific commit (either past or the future)
<<<<<<< HEAD
`$ git reset --hard 09d8c`
 Only first 4-5 chars of commit ID are needed. Can use `$git log` or `$git reflog` to find commit ID. (`$git log --pretty=oneline` to print logs prettier)

Check changes
`$ git diff` 

Delete files
Delete files in working directory
`$ rm <filename>`

Delete files in repo

`$ git rm <filename>`

`$ git commit -m “messages”`

=======
$ git reset --hard 09d8c
 Only first 4-5 chars of commit ID are needed. Can use “$git log” or “$git reflog” to find commit ID. (“$git log --pretty=oneline” to print logs prettier)

Check changes
$ git diff 

Delete files
Delete files in working directory
$ rm <filename>
Delete files in repo
$ git rm <filename>
$ git commit -m “messages”
>>>>>>> dev
