
# Task 10: Comprehensive Workflow with Forced Pushes and Recovery

### 🎯Objective :

- Simulate an advanced Git scenario that includes forced pushes, recovering lost commits, and a multi-branch workflow.


### 📝Steps :

* Create repository with multiple branches

```
    git checkout -b feature1

    git checkout main

    git checkout -b feature2
```

* Do multiple changes and make many commits

* Rebase the changes 

```
    git rebase -i HEAD~3

```
* Force push 

```
    git push origin feature2 --force
```

* Recover lost commits using reflog 

```
    git reflog
    git cherry-pick <commit-hash>
```

#### Caution :
- Git force should be used cautiously because

    * Overwrites history on remote branches
    * Can delete teammates work after you last pull if somebody pushed to remote repo

- Git reflog shows all head movements
    * If accidentally lost a commit during reset or force push `git reflog` will have the commit id as it stores all the head movements.
    * We can use this commit id to `cherry-pick` and add the lost commit on top of our current commit