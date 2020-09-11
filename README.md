# Github-Commands
Terminal Commands for GitHub.  
### I. Adding an existed project to GitHub
1. Create a new repository on GitHub without additional files (like README) added.
2. cd to the current local project folder.
3. Type `git init` to initialize the local directory as a Git repository.
4. Type `git add .` to add all of your files to the staging area and ready to commit.OR type `git add <filename>` to add files one by one. 
5. Type `git commit -m "<add a commit message here>"` to commit. FOR EXAMPLE `git commit -m "First commit"`. 
6. Copy the remote repository URL of the new repo you created in step 1.  
7. Type `git remote add origin <remote repository URL copyed from step 6>` to add the URL for the remote repository where your local repo will be pushed. 
8. Type `git push -u origin master` to push the changes in your local repository to GitHub. 
9. Follow the instruction to type username and password for GitHub.
10. Done!
11. __You can always check changes of your repo with__ `git status`. 

### II. Push local changes to GitHub
If you made some changes to the local repo and want to push it to GitHub:  
1. Type `git status` to see if there are changes made in local repo.  
2. Type `git add .` to add all files.
3. Type `git commit -m "<add a commit message here>"` to commit. 
4. Type `git push` to push changes to GitHub. 

### III. Push local changes to a new branch in GitHub
1. Type `git checkout` to see the current branch you are on.
You can also type `git branch` to see all existing branches.
2. Type `git checkout -b <new_branch_name>` to create a new branch or type `git checkout <existing_branch>` to switch to an existing branch.
3. Type `git status` to check if it is on the right branch. 
4. Type `git add .`. 
5. Type `git commit -m "<add a commit message here>"`. 
6. Type `git push origin <new_branch_name>` to push to the selected branch in GitHub.

### IV. Clone a repo and make changes to original repo
1. Copy the url from the repo in GitHub. 
2. cd to a local project work space.
3. Type `git clone <URL>` in terminal.
4. Make some changes.
5. cd to the local repo folder. 
6. Type `git status` to see if there are changes made in local repo.  
7. Type `git add .`. 
8. Type `git commit -m "<add a commit message here>"`. 
9. Type `git push` to push changes to GitHub. 


### V. Clone a repo and made it my own and has nothing to do with the old one(won't recevie updates from original repo) 
1. Clone the repo you want following step 1 - 3 in last section.
2. Create a new repository in your GitHub without additional files (like README) added and copy the URL. 
3. Type `git remote set-url origin <URL copyed in step 2>`. 
4. Made some local changes. 
5. Type `git status` to see if there are changes made in local repo.
6. Type `git add .`. 
7. Type `git commit -m "<add a commit message here>"`. 
8. Type `git push` to push changes to the repo in your GitHub.

__if you want to receive updates:__   
Use `git remote add personal <URL of your repo>`in step 3.    
__if you want to mannuly receive updates:__  
Use `git remote rename origin upstream` then `git remote add origin <URL of your repo>`. in step 3.   
Type `git push -u origin master` to push the changes to your repository in GitHub for first time. Later you can use `git push`.  
Use `git fetch upstream` when you need to get updates.  
Then type `git checkout master` to switch to master branch.   
Then type `git merge upstream/master` to merge the updates in your repo.   
Fixed any megre error and push into your GitHub.   
