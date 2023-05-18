# advanced1
**Goal**: Rearrange the commits as shown in Goal
```bash
git checkout bugFix
git rebase C2
git checkout C4
git rebase C3'
git checkout C5
git rebase C4'
git checkout side
git rebase C5'
git checkout another
git rebase C6'
git branch -f main C7'
```

# advanced2
## Specifying Parents
**Goal**: Create a new branch at the specified destination
```bash
git checkout HEAD^^2^
git branch bugWork
git checkout main
```
Shortcut
```bash
git branch bugWork HEAD^^2^
```

# advanced3
**Goal**: Update branches **one**, **two** and **three** with modified versions of the last few commits on **main**
```bash
git checkout C1
git cherry-pick C4 C3 C2
git checkout C1
git cherry-pick C5 C4' C3' C2'
git branch -f one C2'
git branch -f two C2''
git branch -f three C2
```