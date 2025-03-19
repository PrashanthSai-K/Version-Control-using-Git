
# Task 4: Simulating and Resolving Merge Conflicts

### 🎯Objective :

- Create a scenario that produces a merge conflict and resolve it.

### 📝Steps :

* Create two branches from the same commit

```
    git checkout -b branch1

    git checkout main

    git checkout -b branch2

```

* Modify the same line in a common file on both branches

* Attempt to merge and observe conflict

```
    git checkout branch1 

    git merge branch2
```

* To inspect the difference 

```
    git diff
```

* Manually resolve the conflict and commit the changes

```
    git add [file]

    git commit -m "Conflict resolved"
```