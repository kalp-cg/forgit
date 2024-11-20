# Part 4: Cherry-Picking Commits (git cherry-pick)
Explanation:- Git cherry pick is command that allows you to apply a specific commit of one branch onto another branch .This is useful when you want to select individual commits from a different branch and bring them into your current branch without merging the entire branch.

=> It is used by git cheery-pick "branch-code"
## Task 8: Pick a Specific Commit
### View the commit history to find the commit hash you want to cherry-pick:
```
git log --oneline
```
### Cherry-pick a specific commit by its hash:
```
git cherry-pick <commit-hash>
```
Example:
```
git cherry-pick e23d8a7
```
Resolve conflicts if any, then commit the changes:
```
git add .
git cherry-pick --continue
```