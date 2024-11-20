# Part 6: Working with Remote Repositories
## Task 12: Add a Remote Repository
### Add a remote repository URL to the project:
```
git remote add origin https://github.com/username/repo.git
```
## Task 13: Fetch Changes from Remote
### Fetch changes from the remote repository without merging them:
```
git fetch origin
```
### View fetched branches:
```
git branch -r
```
## Task 14: Pull Changes from Remote
### Pull the latest changes from the remote repository and merge them into the local branch:
```
git pull origin main
```
## Task 15: Push Changes to Remote
### Push local changes to the remote repository:
```
git push origin main
```
### Push a new branch to the remote repository:
```
git push origin feature-branch
```
## Task 16: Delete Remote Branch
### Delete a remote branch:
```
git push origin --delete feature-branch
```