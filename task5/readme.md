
# Task 5: Interactive Rebasing for Clean Commit History

### 🎯Objective :

- Use interactive rebase to tidy up your commit history.

### 📝Steps :

* Create a series of messy commits

```
    git commit -m "git task 5 modified"

    git commit -m "git task 5 modified.."

```

* Interactive rebase tp tidy up commit history

```
    git rebase -i HEAD~2 //last 2 commits will be rebased

```

* Check if rebase is successfull

```
    git log --oneline
```

#### Squashing

- Squashing will combine multiple commit into one single commit to avoid messier commits and make commits more concise and meaningful to main branch for easier code review