# Part 2: Working with Repositories

## Task 7: Branching and Merging
### 1.Create a new branch for a feature
```
git branch feature_branch
          or
git checkout feature_branch
          or
git checkout -b feature_branch

```
### 2.Add a new file and commit changes:
```
echo "hello world" > file3.txt
git add file3.txt
git commit -m "Newly added"
```

### 3.Merge the feature branch into main
Checkout:- Git checkout is use to create a branch and it is also use to shift to the new branch.
```
git checkout main 
git merge feature_branch
```
Here when we have to merge the feature_branch into main, we have to make sure that the feature_branch is up to date with the main branch. If the feature_branch is not up to date, we have to pull the changes from.

## Task 8: Handeling Merge Conflicts

### 1.Create two branches
```
git branch branch1
git branch branch2
```
### 2.Modify the same line in `README.md` in both branches.

### 3.Merge branch-1 into main
```
git checkout main
git merge branch1
```
### 4.Attempt to merge branch-2 into main (this will cause a conflict)

```
git merge branch2
```

### 5.Resolve the conflict manually in README.md, then
```
git add README.md
git commit -m "Resolved"
```
## Task 9: Renaming and Deleting Branches

### 1.Rename a branch
```
git branch -m old-branch-name new-branch-name
```
### 2.Delete a branch;
```
git branch -d feature_branch

```