# intro1
## Commits
**Goal**: To commit 2 times
```bash
git commit
git commit
```

# intro2
## Branching
**Goal**: To create a new branch *bugFix* and Switch to it
```bash
git branch bugFix
git checkout bugFix
```
Here the First command ***git branch bugFix*** creates a new branch named **bugFix**<br />
The Second command ***git checkout bugFix*** switches to the branch named **bugFix**<br /><br />

Shortcut
```bash
git checkout -b bugFix
```
Here by specifying *-b* argument in the ***git checkout*** command, we just made and switched to branch **bugFix**

# intro3
## Merging
**Goal**
1. Make a new branch called **bugFix**
2. Checkout the **bugFix** branch with ***git checkout bugFix***
3. Commit once
4. Go back to **main** with ***git checkout***
5. Commit another time
6. Merge the branch **bugFix** into **main** with ***git merge***
```bash
git checkout -b bugFix
git commit
git checkout main
git commit
git merge bugFix
```

# intro4
## Rebasing
**Goal**
1. Checkout a branch named **bugFix**
2. Commit once
3. Go back to **main** and commit again
4. Checkout the **bugFix** again and rebase onto **main**
```bash
git checkout -b bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main
```
