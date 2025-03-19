
# Task 6: Stashing Changes for Context Switching


### 🎯Objective :

- Learn how to use Git stash to save uncommitted work temporarily.

### 📝Steps :

* Make changes in working directory

* Stash changes

```
    git stash
```

* Switch branch and perform work

```
    git checkout main
```

* Reapply stashed changes

```
    git checkout feature1

    git stash pop
```

* To view / drop stash

```
    git stash list
    git stash drop stash@{0}
```

### Stash

- Stash takes a snapshot of the current state and store in the stack, successive stash are pushed on top of the stach. Whenever require we can pop or drop the stash whenever required.