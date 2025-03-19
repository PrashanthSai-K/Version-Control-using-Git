
# Task 9: Working with Remote Repositories and Collaboration

### 🎯Objective :

- Simulate a collaborative workflow with remote repositories.

### 📝Steps :

* Create a local repository and push it to a remote

```
    git init
    git remote add origin <remote-repo-url>
    git push -u origin main
```

* Create a feature branch and push

```
    git checkout -b new_feature

    git push origin new_feature

```
* Open a Pull Request in remote repo

* Merge PR and Pull 

```
    git checkout main
    git pull origin main
```