### Basic Info

**Pull all remote changes**

`git fetch --all`

---

**What branch am I on?**

`git branch`

---

**Check Current Status** - current branch - uncommited changes - staged changes - untracked files - branch sync status

`git status`

### Basic Flow

> Clone => Fetch Changes => Create Branch => Add => Commit => Push

**Clone repo to current folder**

```
# clone to current folder
git clone <repository-url>

# clone and specify folder name (insted of repo name)
git clone <repo-url> <folder-path>
```

---

**Create New Branch**

```
git checkout -b <branch-name>
```

---

**Publish new branch and set upstream origin**

```
git push -u origin <branch-name>
```

'**-u**' sets tracking to the upstream origin. This is only needed when first publishing a new branch on the first push. If you create a branch on github, or use VS Code UI "create branch", this is not needed.

---

**Stage all Changes**

```
git add .
```

---

**Commit**

```
git commit -m "your commit message"
```

---

**Push**

```
git push
```

### Undo a commit

**1. Undo commit and unstage changes**

```

git reset HEAD~1
```

---

**2. Undo commit and discard changes**

```
git reset --hard HEAD~1
```

---

**3. Undo a pushed commit (creates new commit)**

```
git revert HEAD
```
