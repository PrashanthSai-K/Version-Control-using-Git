
# Task 2: Gitignore and Tracking Files

### 🎯Objective :

- Set up a `.gitignore` file to exclude certain files or directories.
- Verify that ignored files are not tracked by Git.

### 📝Steps :

  * Create `.gitignore` with required patterns

```
*.log
*.env

node_modules/
build/
```

* Add files like .env, .log to test ignore patterns

* Check status

```
git status
```
* Only gitCommands.txt is tracked, others are ignored


