# Initialize A Folder (for Mac Terminal)

cd ~/Desktop

git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_FOLDER_NAME.git

cd YOUR_FOLDER_NAME

  #now you have a folder on the desktop, connected to your github


# Add/Check Remotes
### make sure you are in the github connected folder
git remote -v
### add a "upstream" remote, and check

git remote add upstream https://github.com/ANOTHER_GITHUB_USERNAME/ANOTHER_FOLDER_NAME.git

git remote -v

# Update Your Fork

### check your branch
git branch

git checkout master

### pull "upstream" content to local
git fetch upstream

git pull upstream master
### push local content to "origin"
git push origin master


# Update Local Changes to Github

### add new files
git add .

### commit new files
git commit -m "your message"

### update github
git push origin master


# Mandatorily Overwrite Local Folder (when necessary)
git fetch upstream

git checkout master

git reset --hard upstream/master

git push origin master --force


# Track Changes

### see history of commit messages
git log

### detect changes
git status

git diff


# Other Comments

### References

https://github.com/prof-rossetti/nyu-info-2335-70-201706/blob/master/notes/git/cli.md
https://github.com/Cynthia0524/nyu-info-2335-70-201706/blob/master/CONTRIBUTING.md

### upstream and origin could be exchanged
