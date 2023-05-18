# remoteAdvanced1
## Merging feature branches
**Goal**
1. There are three feature branches -- **side1**, **side2** and **side3**
2. We want to push each one of these features, in order, to the remote
3. The remote has since been updated, so we will need to incorporate that work as well
```bash
git checkout main
git pull
git cherry-pick C2 C3 C4 C5 C6 C7
git branch -f side1 C2'
git branch -f side2 C4'
git branch -f side3 C7'
git push
```

# remoteAdvanced2
## Merging with remotes
**Goal**
1. There are three feature branches -- **side1**, **side2** and **side3**
2. We want to push each one of these features, in order, to the remote
3. The remote has since been updated, so we will need to incorporate that work as well
```bash
git checkout main
git pull
git merge C2
git branch -f main C4
git merge C9
git branch -f main C7
git merge C10
git push
```

# remoteAdvanced3
## Remote Tracking
**Goal**: push work onto the main branch on remote while not checked out on main locally
```bash
git checkout -b side o/main
git commit
git fetch
git checkout o/main
git cherry-pick side
git branch -f side C3
git checkout side
git push
```

# remoteAdvanced4
## Push Arguments
**Goal**: update both **foo** and **main** on the remote
```bash
git push origin main
git push origin foo
```

# remoteAdvanced5
## Argument Details (colon refspec)
**Goal**: Get to the end goal state shown in the visualization
```bash
git push origin main^:foo
git push origin foo:main
```

# remoteAdvanced6
## Git Fetch Arguments
**Goal**: fetch the specified commits in the goal visualization
```bash
git fetch origin main^:foo
git fetch origin foo:main
git checkout foo
git merge C6
```

# remoteAdvanced7
## Source of Nothing
**Goal**: delete one remote branch and create a new branch
```bash
git push origin :foo
git fetch origin :bar
```

# remoteAdvanced8
## Pull Arguments
**Goal**: download some commits, make some new branches, and merge those branches into other branches
```bash
git pull origin bar:foo
git pull origin main:side
```