
# Git Commands

```bash
git init # This will create a .git folder in the project 
```

```jsx
git remote add origin [https://github.com/username/repository.git](https://github.com/username/repository.git) # To set remote
```

git remote show origin

# 

```jsx
git remote show origin
# Following comments shows example output
#remote origin
#Fetch URL: [git@github.com](mailto:git@github.com):shashankyld/orbslam3_ROS.git
#Push URL: [git@github.com](mailto:git@github.com):shashankyld/orbslam3_ROS.git
#HEAD branch: (unknown)
```

```bash
git status # This will show all the changes that happened so far  
```

```bash
git add . # This will stage all the files in the cwd to be commited
```

```bash
git add <filename? # One can also stage individual files
```

```bash
git commit -m "ADD A MESSAGE THAT SUMMARIZE THE COMMIT" 
# This will commit the changes and adds a message
```

```bash
git restore --staged <filename> 
# This will remove the file from the stage and move back to the unstaged
```

```bash
git reset <commit id> 
# This will remove all the commits that are done after this commit 
# The deleted commits will go to the unstaged area
# You can check using 
git status
```

```bash
# Use this in case you deleted commits by mistake
git restore <filename>
# This will discard changes in the working directory 
```

```bash
# If you dont want to commit a few staged changes for now temporarily
# We can send these commits "backstage" for them to be popped back later
git stash # This will hide staged changes temporarily

# To bring back those backstaged changes, use
git stash pop # This will stage the hidden changes again

# If we choose to delete these backstaged changes, use
git stash clear # This will clear all the stash entries

```

```jsx
git push origin master # Push
```
