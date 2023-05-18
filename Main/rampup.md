# rampup1
## Head
**Goal**: Detach *Head* from **bugFix** and attach it to commit **C4**
```bash
git checkout C4
```

# rampup2
## Relative Ref
**Goal**: Checkout parent commit of **bugFix**
```bash
git checkout bugFix^
```

# rampup3
## Relative Ref (Moving a Branch to a specific commit)
**Goal**: Move **head**, **main** and **bugFix** to their goal destinations shown
```bash
git branch -f main C6
git branch -f bugFix HEAD~2
git checkout C1
```
# rampup4
## Reverse changes in Git
**Goal**: Reverse the most recent commit on both **local** and **pushed**
```bash
git branch -f local HEAD^
git checkout pushed
git revert pushed
```
### Note
**pushed** is a remote branch
**local** is a local branch
