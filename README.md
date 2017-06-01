# Exercises
## 1. Starting from scratch

### 1.1 Create a new git repository  
Create an empty folder, and a new git repository within it.

### 1.2 Add README to the repository
1. Create a new README file, and add some content there (a triceratops maybe?). 
2. Make a new commit containing the file, with appropriate commit message.  

### 1.3 Create a repository in Github and push the local repo there
1. Create a new repository in Github (https://github.com/new), with **no** .gitignore, LICENSE or README files.
2. Set the repository address as a remote for the local git repo
3. Push the local repo to the remote Github repo

## 2 Working with history

### 2.1 More history pls!
1. Make two more commits, which contain changes to existing files, or creation of new files.

### 2.2 Inspect all of the history
1. Inspect the commit log using the appropriate git command

### 2.3 Inspect only parts of the log
1. Use git commit syntax to inspect log with
    - Only the latest commit (HEAD of the branch)
    - Two of the latest commits
    - Commits from COMMIT_X to COMMIT_Y
    - Commits from COMMIT_X (excluding) to COMMIT_Y
    
### 2.4 Revert changes
1. Revert changes applied in 2.1., without removing the commits
2. Remove the commit made in the previous step

## 3 Merging and branching

### 3.1. Basic branching
1. Create a new branch
2. Start working on that branch

### 3.2. Cause a conflict
1. Modify a line on one of the existing files in the new branch
2. Commit the changes
3. Modify the **same** line on the master branch
4. Commit also those changes
5. Go back to the new branch
6. Merge master branch to the new branch
7. Resolve the conflict.

### 3.3 Bring your changes back to master
1. Merge your new branch to master
2. Push the changes to origin/master

## 4 Github workflow

### 4.1 Clone the repo
1. Clone this repo to some folder on your computer

### 4.2 Create a branch within Github
1. Create branch called `yourfirstnamelastname` within Github  
![Branching](/refpics/github-branching.png)

2. Create a local branch from this remote branch, and start using it
```bash
git fetch # fetch new changes from upstream (Github) but don't merge anything
git remote -r # List all remote (Github) branches. You should see origin/yourfirstnamelastname
git checkout origin/yourfirstnamelastname -b local-branch-name
```

3. Move your picture from gitnoobs folder to gitmasters folder
4. Commit the change, and push it to your remote branch (**NOT MASTER**)
5. Create a pull request on Github