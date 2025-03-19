
# Task 8: Using Git Hooks for Automated Checks


### 🎯Objective :

- Set up a Git hook to run scripts (like linters or tests) before commits are finalized.

### 📝Steps :

* Create a `pre-commit` hook in `.git/hooks` folder

* Sample hook script 

```
#!/bin/sh
#
echo "Linting files......"

FILES=$(git diff --cached --name-only -- '*.js')

if [ $FILES = "" ]; then
	echo "No JS files found to lint"
	exit 0
fi

npx eslint $FILES

if [ $? -ne 0 ];then
	echo "❌ Linting failed. Please fix the issues before committing."
	exit 1
fi

echo "✅ Linting passed!"
exit 0

```

* Create a sample js file and commit to check if pre-commit script works fine.