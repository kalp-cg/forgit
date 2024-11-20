# Part 3: Interactive Rebase (git rebase -i)
## Task 6: Use Interactive Rebase to Modify Commit History
### View the last few commits:
```
git log --oneline
```
### Start an interactive rebase for the last 3 commits:
```
git rebase -i HEAD~3
```
Explanation: This opens an editor with the list of commits in the last 3 commits.
Modify the commits by changing pick to one of the following:

squash (combine commits)
reword (edit commit message)
edit (edit commit content)
drop (remove commit)
Example of squashing two commits:

Change the second commit from pick to squash and save.
Git will combine the commit messages for the squashed commit.

## Task 7: Complete Interactive Rebase
After modifying the commits, save and close the editor.
Resolve any conflicts if prompted, then continue the rebase:
```
git rebase --continue
```