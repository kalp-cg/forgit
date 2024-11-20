# Part 8: Automation and Cleanup
## Task 19: Cleaning the Repository
### Remove untracked files:
```
git clean -f
```
## Task 20: Aliases and Shortcuts
### Create an alias for frequently used commands:

```
git config --global alias.st status
git config --global alias.cm commit
```
### Use the alias:
```
git st
git cm -m "Message"
```