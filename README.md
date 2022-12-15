# Git Commands

Important steps for git workflow:

### Create a new repo in the command line:
*Make a directory. Be sure you are in your home directory first.*</br>
  $ mkdir repo_name</br>
*Move into your new directory (or repo)*</br>
  $ cd repo_name</br>
*Add README.md file (also adding a simple comment (# README #)*</br>
  $ echo '# README #' > README.md</br>
*Add LICENSE.md file (also adding a simple comment (# LICENSE #)*</br>
  $ echo '# LICENSE #' > LICENSE.md</br>
*Add .gitignore file **SHOULD BE CREATED FOR ALL REPOS** (holds data you don't want to be shared)*</br>
  $ touch .gitignore</br>
*Check to make sure all files were added into repo_name*</br>
  $ ls -a</br>
*Make sure your primary branch in GitHub uses "main" (only need to do this step if setting up GitHub for the first time)*
</br>
  $ git config --global init.defaultBranch main</br>
  
### Initialize a new repo in your current directory. 
**IMPORTANT YOU ARE IN THE DIRECTORY YOU WANT TO INITIALIZE AS A REPO** </br>
  $ git init</br>
  Initialized empty Git repository in .../repo_name/.git/</br>
  (.git directory will be added to your new repository. It can be deleted if you accidentally initialize in the wrong directory.)</br>
Check status of those files with git status</br>
  $ git status</br>
Stage changes for commit</br>
  $ git add .  </br>
  (can check status again. You should see the files are staged, ready to be committed)</br>
Commit changes to version history</br>
  $ git commit -m 'Add first project files'</br>
Review previous changes with git log</br>
  $ git log</br>
  
### Push code to GitHub
  $ git push origin main</br>
  $ git push origin main -ff (if you are getting an error about fast-forwards)</br>
  
### Pull code from GitHub
  $ git pull origin main (if you are getting an error about failing to push some refs)</br>
    -after you pull the code, commit it again and then push it back to GitHub</br>
    
### Add local repo to remote repo
  $ git remote add origin https://github.com/username/repo_name
