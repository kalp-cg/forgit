# Part-1 Understanding and Using git stash
## Task 1: Save Changes Temporarily with git stash
<!-- When we apply changes into the file without committing -->

### Create a new file
```
echo "Creating new file..." >> temp-file.txt
```
### View tracked and untracked files
```
git status
```    
### Stash the changes:
```
git stash
```   
### View all stashes as a list format
```
git stash list
``` 

## Task 2: Apply and Drop Stashed Changes
### To apply recently added stash:
```
git stash apply
```   
### To drop recently added stash after applying
```
git stash drop
```   
### When we need to apply a specific stash:
```
git stash apply stash@{1}
```   
## Task 3: Stash Untracked Files

### Stash changes, including untracked files:
```
git stash -u
```
### To apply stashed changes including untracked files:
```
git stash apply
```