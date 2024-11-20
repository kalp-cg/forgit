# Part 3: Branching and Merging
## Task 6: Branch Management
### Create a branch and switch to it:
```
git checkout -b feature-branch
```
### List branches:
```
git branch
```
### Rename a branch:
```
git branch -m feature-branch feature-enhanced
```
## Task 7: Merging Branches
### Merge feature-enhanced into main:
```
git checkout main
git merge feature-enhanced
```
## Task 8: Handling Merge Conflicts
### Create two conflicting branches and resolve a conflict manually:
```
git merge <branch-name>
Use:
git add <resolved-file>
git commit
```