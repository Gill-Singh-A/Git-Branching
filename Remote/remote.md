# remote1
## Clone<br />
**Goal**: Clone a Git Repository
```bash
git clone
```

# remote2
## Git Remote Branches<br />
**Goal**: Commit once off of **main** and once after checking out **o/main**
```bash
git commit
git checkout o/main
git commit
```

# remote3
## Git Fetch<br />
**Goal**: Simply git fetch and download all the commits
```bash
git fetch
```

# remote4
## Git Pull<br />
**Goal**: 
```bash
git pull
```

# remote5
## Git fakeTeamwork
**Goal**: Make a remote (with git clone), fake some changes on that remote, commit yourself, and then pull down those changes
```bash
git clone
git fakeTeamwork 2
git commit
git pull
```

# remote6
## Git Push
**Goal**: Share two new commits with the remote
```bash
git commit
git commit
git push
```

# remote7
## Diverged History
**Goal**
1. Clone your repo
2. Fake some teamwork (1 commit)
3. Commit some work yourself (1 commit)
4. Publish your work via rebasing
```bash
git clone
git fakeTeamwork
git pull --rebase
git push
```

# remote8
## Pull Requests
**Goal**: Create another branch called feature and push that to the remote
```bash
git branch -f main C1
git checkout -b feature
git branch -f feature C2
git push
```
