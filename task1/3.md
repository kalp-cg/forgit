# Part 3: Advanced Git Operations

## Task-10: Using Git stash

### 1.Make changes to a file but don’t commit:
```
echo "Temporary work" >> temp.md
```

### 2.Stash the changes:
Git stash:- Git stash is a command which is use when we work on repo and we do some changes but we don’t want to commit those changes and don't want to delete that changes at that time we use stash command. In stash command this all changes are save and we requir at that time we use it.
```
git stash
```

### 3.View stashed changes:
```
git stash list
```

### 4.Apply the stashed changes:
```
git stash Apply
```
### 5.Drop the stash after applying:
Git stash drop:- This command removes the most recent stash from the stash list:
```
git stash drop
```
# Part 3: Advanced Git Operations
## Task 10: Using Git Stash
### Make changes to a file but don’t commit:
```
echo "Temporary work" >> temp.md
```
### Stash the changes:
```
git stash
```
### View stashed changes:
```
git stash list
```
### Apply the stashed changes:
```
git stash apply
```
### Drop the stash after applying:
```
git stash drop
```
## Task 11: Rewriting History with Interactive Rebase
### Create multiple commits:
```
echo "Commit 1" > file1.txt && git add file1.txt && git commit -m "Commit 1"
```
```
echo "Commit 2" > file2.txt && git add file2.txt && git commit -m "Commit 2"
```
```
echo "Commit 3" > file3.txt && git add file3.txt && git commit -m "Commit 3"
```

### Squash commits into one:
```
git rebase -i HEAD~3
```
Example: Replace pick with squash for the second and third commits.

## Task 12: Cherry-Picking Commits
### Create a new branch:
```
git checkout -b cherry-pick-example
```

### Cherry-pick a specific commit from another branch:
```
git cherry-pick <commit-hash>
```
## Task 13: Tagging Commits
### Tag the current commit:
```
git tag -a v1.0 -m "Version 1.0 release"
```

### Push the tag to the remote repository:
```
git push origin v1.0
```
## Task 14: Working with Remote Repositories
### Add a remote repository:
```
git remote add origin <repository-url>
```
### Push your changes to the remote repository:
```
git push origin main
```
## Task 15: Forking and Contributing
### Fork a repository on GitHub.

### Clone the fork locally:
```
git clone <forked-repo-url>
```
### Create a new branch, make changes, and push:
```
git checkout -b fix-typo
echo "Typo fixed" >> README.md
git add README.md
git commit -m "Fixed a typo"
git push origin fix-typo
```

Open a pull request on GitHub.