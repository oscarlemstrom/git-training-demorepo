# Exercises
## 1. Starting from scratch

### 1.1 Create a new git repository  
1. Create an empty folder, and a new git repository within it.

### 1.2 Add README to the repository
1. Create a new README file, and add some content there (a triceratops maybe?). 
2. Make a new commit containing the file, with appropriate commit message.  

### 1.3 Create a repository in Github and push the local repo there
1. Create a new repository in Github (https://github.com/new), with **no** .gitignore, LICENSE or README files.
2. Set the repository address as a remote for the local git repo
3. Push the local repo to the remote Github repo

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

### 4.3. Make a pull request
1. Move your picture from gitnoobs folder to gitmasters folder. If your picture is not there (new peeps sorry :<), feel free to add any other image to the gitmasters folder
2. Commit the change, and push it to your remote branch (**NOT MASTER**)
3. Create a pull request on Github  
![Pull request](/refpics/github-prs.png)  
![Comparison](/refpics/github-comparison.png)