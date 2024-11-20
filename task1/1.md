# Part-1
## Task 1: Install and Configure Git
### 1.Configure Git with your username and email:
Git config is a git command which is used to cofigure git setting. These settings can control various aspects of how Git behaves, Git username, useremail,file handeling,merge behaviours. This configurations can be set at three diffrent levels.

1-Local.
=>This setting is only applicable to the local repository or the repository on which we are working.

2-Global.
=>Specific to the current user. This setting is applicable to all the repositories on the local machine and in our account.

3-System.
=>Specific to the entire system (for all users). These settings are stored in a system-wide configuration file

```
git config --global user.name"Jatin"
git config --global user.email"Jatin@gmail.com"
```

### 2.View your Git configuration:
We can check our confriguration by using the following command:
```
git config --list
```

## Task 2: Initialize a Repository

### 1.Create a new project folder and navigate to it:
Git init means to initialize a new git repository to do a git work on it like git add,git commit,git push etc.

```
mkdir myproject
cd myproject
```
### 2.Initialize it as a Git repository:
```
git init
```
Example:
After running git init, a hidden .git folder will appear in the directory, indicating it’s now under version control.

## Task 3: Create a File and Make Multiple Commits

### 1.Create a new file and add content:
For Creating a new file using echo we use a echo in which when we use ">" greater than sign means we are creating a new file and when we use ">>" double greater than sign means we are going to append(add some content) the content in the existing file
```
echo "Hello world" >> file.txt
```

### 2.Stage the file
Staging the file means to add the file.

```
git add file.txt
```
### 3.Commit the file 
 Commit means to save the file after adding it with some meassge.

 ```
 git commit -m "First commit"
 ```

### 4.Make changes to the file
Here during making the or during adding the file we have to take the note [>] one greater thean is use to make the make the file, while [>>] two greater than is use to add an modify the file.

```
echo  "Hello eveyone" >> file.txt
```

### 5.Stage the file and commit the changes
git add file.txt
git commit -m "Second commit"

## Task 4: Check Status and Log
git status: - Git status is use to dee that what is the status of the file is it added or not.
git log: -git log is used to see the 
### 1.Check the repository’s current status
git status

### 2.View commit history in detail:

``` 
git log --oneline --graph --decorat
```

git log --oneline --graph --decorate is a graph Draw a text-based graphical representation of the commit history on the left hand side of the output.

## Task 5: Create a clone and repository
git clone: - git clone is used to create a copy of the repository.
1.Create a repository on GitHub named `example-repo`.

2.Clone it locally:
git clone http://codinggita.com/ex.repo

## Task 6:  Understanding the Git Workflow

Example Workflow

i. Make changes to a file in the working directory:
```
echo "hello world" > file2.txt
```

ii.Stage the file:
```
git add file2.txt
```

iii commit the file to the repository;
```
git commit -m "first new commit"
```