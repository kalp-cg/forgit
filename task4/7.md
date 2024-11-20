
# Part 7: Forking and Contributing to Open-Source Projects
## Task 17: Fork a Repository on GitHub
### Go to a repository on GitHub and click Fork in the top right corner to create your own copy of the repository.

### Clone the forked repository to your local machine:
```
git clone https://github.com/your-username/repo.git
```
## Task 18: Make Changes and Commit
Create a new branch for your changes:
```
git checkout -b fix-typo
```
### Make changes to the code (e.g., fix a typo in README.md), stage, and commit them:
```
git add README.md
git commit -m "Fixed typo in README.md"
```
## Task 19: Push Changes to Your Fork
### Push the changes to your remote fork:
```
git push origin fix-typo
```

## Task 20: Create a Pull Request
Explanation Of Pull Request:- Pull request means when someone make a new  branch in our repo and they do a work on it. After sometime they want to merge their branch with our main branch. So they create a pull request and ask an owner of main branch to review and merge that merge branch in main branch.

### Go to your forked repository on GitHub, click on Compare & Pull Request.
### Write a description of your changes and submit the pull request to the original repository.
## Task 21: Sync Your Fork with the Original Repository
### Add the original repository as a remote source:
```
git remote add upstream https://github.com/original-owner/repo.git
```
### Fetch changes from the original repository:
```
git fetch upstream
```
### Merge changes from the original repository into your local branch:
```
git checkout main
git merge upstream/main
```
### Push the changes to your fork:
```
git push origin main
```