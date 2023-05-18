# mixed1
## Locally Stacked Commits
**Goal**: To Rebase the Final Commit of **bugFix** onto **main**
```bash
git rebase -i HEAD~3
git branch -f main C4'
```

# mixed2
## Juggling Commits
**Goal**: Re-order commits as shown in Goal
```bash
git rebase -i HEAD~2
git rebase -i HEAD^
git rebase -i HEAD~2
git branch -f main C3''
```

# mixed3
## Juggling Commits
**Goal**: Re-order commits as shown in Goal (without using *rebase -i*)
```bash
git rebase -i HEAD~2
git rebase -i HEAD^
git cherry-pick C3
git branch -f caption C3
git branch -f main C3'
```

# mixed4
## Git Tags
**Goal**: Create the tags in the goal visualization and then check **v1** out
```bash
git tag v0 c1
git tag v1 c2
git checkout v1
```

# mixed5
## Git Describe
**Goal**: Describing a few of the locations
```bash
git commit
```
