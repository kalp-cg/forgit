# Part 5: Advanced Git
## Task 12: Stashing Changes
### Save uncommitted changes:
```
git stash
```
### Apply stashed changes:
```
git stash apply
```
### Drop the stash:
```
git stash drop
```
## Task 13: Tagging Commits
### Create and annotate a tag:
we use the git tag command to create a tag. The -a option is used to create an annotated tag, and the
```
git tag -a v1.0 -m "Version 1.0 release"
```
### Push the tag to the remote:
```
git push origin v1.0
```

## Task 14: Rewriting Commit History
### Use interactive rebase to modify commit messages:
In git rebase when we do a git rebase at that time all the commit of feature branch is merge with main branch and additional commit is not formed.

```
git rebase -i HEAD~3
```
Replace pick with edit or squash as needed.

### Task 15: Cherry-Picking Commits
Apply a specific commit to another branch:
```
git cherry-pick <commit-hash>
```