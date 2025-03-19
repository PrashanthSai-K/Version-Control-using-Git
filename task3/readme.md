
# Task 3: Undoing Changes and Reverting Commits

### 🎯Objective :

- Experiment with undoing changes in your working directory and commits.

### 📝Steps :

* Modify a tracked file

* Undo changes using `git checkout -- [filename]`

* Make a commit

* Undo commit using revert to change back to any old commit by creating a new commit

```
    git revert b9477d9f7dc95ff3dc60642a62ab74c6c7796ce0 //commit hash
```

* Undo commit using reset to change back to any old commit by going back to the commit (unstaged) 

```
    git reset a4f5b7c10114dd6c56aa0cd35d89e1b9e5b221e5
```

* If hard flag is used, then well go back to the commit by wiping out the changes (Dangerous)

```
    git reset --hard a4f5b7c10114dd6c56aa0cd35d89e1b9e5b221e5 
```

### Difference between `revert` and `reset` :

* `git revert` will create a new commit when undoing changes
* `git reset` will move the HEAD(pointer) to previous commit (will likely to change commit history)