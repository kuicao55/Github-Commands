# Github-Commands
Terminal Commands for GitHub.  
### Adding an existed project to GitHub
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

### Push local changes to GitHub
If you made some changes to the local repo and want to push it to GitHub:  
1. Type `git status` to see if there are changes made in local repo.  
2. Type `git add .` to add all files.
3. Type `git commit -m "<add a commit message here>"` to commit. 
4. Type `git push` to push changes to GitHub. 

