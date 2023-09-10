
<span style="font-family: 'Poppins', sans-serif;">

# Introduction 💖
This guide should help you navigate through Git and GitHub efficiently. Happy coding!

> `Author:` Asif Shahzad <br>

> `Contact Me:` +92 310 6715784

## Basic Commands

### Create a File
```bash
$ touch filename.extension
```

### Open a Plain Text File
```bash
$ nano filename
```
- `nano` is a command-line text editor similar to notepad in a graphical interface.

### `nano` Editor Important Key Combinations

- Press <kbd>CTRL + O</kbd> and then enter to *Save a File*.
- Press <kbd>CTRL + X</kbd> to *Exit* from the editor.

## File Operations

### Show Files in a Directory
```bash
$ ls
```

### Change Directory
```bash
$ cd <directory name>
```

### Show Current Location
```bash
$ pwd
```

### Go One Step Back into Directory
```bash
$ cd -  # or cd ..
```

### Go Two Steps Back into Directory
```bash
$ cd --  # or cd ../..
```

### List Files (Including Hidden)
```bash
$ ls -lart
```
### Remove a File or Directory

- Remove a file: `$ rm filename`
- Remove a directory: `$ rm -r directoryname`



## Check Git Version
```bash
$ git --version
```

## Configuration: Name and Email
```bash
$ git config --global user.email "youremail@example.com"
```
```bash
$ git config --global user.name "Your Name"
```

## Check Configured User
```bash
$ git config --global --list
```

## Initialization to Git
```bash
$ git init
```



# Working and Staging

## Staging Area

If you're working with `file1` and `file2` and you only want to upload or save changes made to `file1`, you can use the staging area. It's a place to save your changes for later upload, like posing for a photo.

## Working Area

This is where you do your work before saving it to the staging area.

## Modified File

Files in red after `git status` are modified.

## Tracked File

Files already uploaded in Git are displayed in green.

### Git Status
```bash
$ git status
```

### Move to Staging Area
```bash
$ git add <file name>
```

### Stage All Modifications
```bash
$ git add .  # or $ git add -A
```

### Commit
```bash
$ git commit -m "Your Message"
```

### Create New File Using Terminal
```bash
$ touch <file name>
```

### Git Checkout
```bash
$ git checkout <filename>
```

### Git Log
```bash
$ git log
```

### View Specific Number of Logs
```bash
$ git log -p -5  # Display last five commits
```

### Git Diff
```bash
$ git diff  # Compare working area with staging area
$ git diff --staged  # Compare staging area with last commit
$ git checkout -f  # Remove changes from last commit
```

# Git Ignore

`.gitignore` is used to ignore files from being committed.

- Ignore specific file: `FILENAME.EXTENSION`
- Ignore all files with a particular extension: `*.EXTENSION`



# Git Branches

#### Create a Branch
```bash
$ git branch <branchname>
```

#### Switch to a Specific Branch
```bash
$ git checkout branchname
```

#### Create and Switch Branch Simultaneously
```bash
$ git checkout -b branchname
```

#### View Branches
```bash
$ git branch
```

#### Merge Git Branches
```bash
$ git merge feature1
```

---

# Remote Repository

To push code online, you need a GitHub repository (remote repo) where you can store your code.

## Setting Remote Repo
```bash
$ git remote add origin <repo-url>
```

## Update Existing Remote URL
```bash
$ git remote set-url origin ssh-url
```

## Pushing Code into Remote Repo
```bash
$ git push -u origin master
```

1. **`git push`**: Command used to send local changes to a remote location.

2. **`-u`**: Stands for "upstream", tells Git to remember the details of this remote location (`origin`) and the branch (`master`). So, in the future, when you run `git push`, Git will know where to send your changes.

3. **`origin`**: The name given to the remote repository.

4. **`master`**: The name of the branch you're pushing.


</span>

