# Git Commands

Important steps for git workflow:

## Create a new repo in the command line:
Make a directory. Be sure you are in your home directory first.
  $ mkdir repo_name
Move into your new directory (or repo)
  $ cd repo_name
Add README.md file (also adding a simple comment (# README #)
  $ echo '# README #' > README.md
Add LICENSE.md file (also adding a simple comment (# LICENSE #)
  $ echo '# LICENSE #' > LICENSE.md
Add .gitignore file **SHOULD BE CREATED FOR ALL REPOS** (holds data you don't want to be shared)
  $ touch .gitignore
Check to make sure all files were added into repo_name
  $ ls -a
Make sure your primary branch in GitHub uses "main" (only need to do this step if setting up GitHub for the first time)
  $ git config --global init.defaultBranch main
  
## Initialize a new repo in your current directory. **IMPORTANT YOU ARE IN THE DIRECTORY YOU WANT TO INITIALIZE AS A REPO** 
  $ git init
  Initialized empty Git repository in .../repo_name/.git/
  (.git directory will be added to your new repository. It can be deleted if you accidentally initialize in the wrong directory.)
Check status of those files with git status
  $ git status
Stage changes for commit
  $ git add .
  (can check status again. You should see the files are staged, ready to be committed)
Commit changes to version history
  $ git commit -m 'Add first project files'
Review previous changes with git log
  $ git log
  
## Push code to GitHub
  $ git push origin main
  $ git push origin main -ff (if you are getting an error about fast-forwards)
  
## Pull code from GitHub
  $ git pull origin main (if you are getting an error about failing to push some refs)
    -after you pull the code, commit it again and then push it back to GitHub
    
## Add local repo to remote repo
  $ git remote add origin https://github.com/username/repo_name
