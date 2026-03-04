### Basic Info

**Pull all remote changes**

```git
git fetch --all
```

**What branch am I on?**

```
git branch
```

**Git Status**

- current branch
- uncommited changes
- staged changes
- untracked files
- branch sync status

```git
git status
```

### Basic Flow

**Clone repo to current folder**

```
# clone to current folder
git clone <repository-url>

# clone and specify folder name (insted of repo name)
git clone <repo-url> <folder-path>
```

**create new branch**

```
git checkout -b <branch-name>
```

**publish new branch and set upstream origin**

```
git push -u origin <branch-name>
```

**stage all changes**

```
git add .
```

**commit**

```
git commit -m "your commit message"
```

**Push**

```
git push
```

### Undo a commit

**1. Undo commit and unstage changes**

```

git reset HEAD~1
```

**2. Undo commit and discard changes**

```
git reset --hard HEAD~1
```

**3. Undo a pushed commit (creates new commit)**

```
git revert HEAD
```

lets push a mistake a revert it
