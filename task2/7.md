# Part 7: Ignoring Files
## Task 18: Using .gitignore
### Create a .gitignore file:
```
echo "node_modules/" > .gitignore
git add .gitignore
git commit -m "Added .gitignore"
```
### Verify that ignored files are not staged:
```
git status
```