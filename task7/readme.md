
# Task 7: Cherry-Picking Commits Between Branches


### 🎯Objective :

- Selectively apply a commit from one branch to another using cherry-pick.

### 📝Steps :

* Create two branches with distinct commits

```
git checkout -b branch1
git commit -m "change 1"

git checkout main

```

* Identify commit to cherry-pick

```
    git log --oneline

```

* Cherry-pick commit

```
    git checkout main

    git cherry-pick c185172
```

* Verify if commit applied

```
    git log --oneline
```