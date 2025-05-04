# 🐧 Linux & Git Cheatsheet

*A quick reference for common terminal commands every developer must know.*

---

## 🔍 BASIC NAVIGATION

### `pwd` (Print Working Directory)
**What it does**: Shows the full path of your current folder.  
**When to use**: To confirm where you are in the file system.
```bash
pwd
# Output: /home/godsfavour/projects/ngswap
```

### `cd` (Change Directory)
**What it does**: Moves you to a different folder.  
**When to use**: To navigate between project folders or system directories.
```bash
cd Documents/roetechhub
cd ..       # Go up one level
cd ~        # Go to home directory
cd /        # Go to root of file system
```

---

## 📁 FILE & DIRECTORY MANAGEMENT

### `ls` (List)
**What it does**: Lists files and folders in the current directory.  
**When to use**: To see what's inside a directory.
```bash
ls          # Simple list
ls -l       # Long format with permissions
ls -a       # Shows hidden files (starts with .)
```

### `mkdir` (Make Directory)
**What it does**: Creates a new folder.  
**When to use**: To organize files into directories.
```bash
mkdir ngswap
mkdir -p ngswap/src/assets # Create nested folders in one command
```

### `touch` (Create File)
**What it does**: Creates an empty file.  
**When to use**: To make placeholder files for code, configs, etc.
```bash
touch index.html
touch script.js README.md
```

### `rm` (Remove)
**What it does**: Deletes files or folders (use with caution).  
**When to use**: To clean up or delete unnecessary files.
```bash
rm file.txt             # Delete file
rm -r old_folder        # Delete folder and contents
rm -rf node_modules/    # FORCE delete folder (no confirmation)
```

### `cp` (Copy)
**What it does**: Copies files or directories.  
**When to use**: To duplicate files or backup configs.
```bash
cp index.html backup.html
cp -r my_folder/ backup_folder/
```

### `mv` (Move/Rename)
**What it does**: Moves or renames files/folders.  
**When to use**: To organize or rename your files.
```bash
mv logo.png assets/logo.png
mv oldname.html newname.html
```

---

## 🛠️ SYSTEM UTILITIES

### `clear`
**What it does**: Clears the terminal screen.  
**When to use**: When your terminal is cluttered.
```bash
clear
```

### `exit`
**What it does**: Closes the terminal or ends an SSH session.
```bash
exit
```

### `history`
**What it does**: Shows previously entered commands.
```bash
history
```

---

## ⚙️ PERMISSIONS & EXECUTION

### `chmod` (Change Mode)
**What it does**: Changes file or script permissions.  
**When to use**: To make files executable.
```bash
chmod +x install.sh     # Give execute permission
chmod 755 script.sh     # Set read/write/execute for owner, read/execute for others
```

### `sudo` (Superuser Do)
**What it does**: Runs a command with administrator privileges.  
**When to use**: For system-level changes (installing software, editing system files).
```bash
sudo apt update
sudo nano /etc/hosts
```

---

## 🌐 NETWORKING

### `ping`
**What it does**: Tests internet or server connection.
```bash
ping google.com
```

### `ifconfig` or `ip a`
**What it does**: Shows your machine’s network IP settings.
```bash
ip a
```

---

## 🌳 GIT VERSION CONTROL

### `git init`
**What it does**: Initializes a new Git repository in your current folder.
```bash
git init
```

### `git add`
**What it does**: Stages changes for commit.  
**When to use**: After editing or creating files.
```bash
git add .        # Stage all changes
git add index.js # Stage specific file
```

### `git commit -m "message"`
**What it does**: Saves a snapshot of staged changes.
```bash
git commit -m "Added homepage layout"
```

### `git status`
**What it does**: Shows the state of your working directory and staged files.
```bash
git status
```

### `git log`
**What it does**: Displays commit history.
```bash
git log --oneline
```

### `git clone`
**What it does**: Copies a remote repo to your local machine.
```bash
git clone https://github.com/username/project.git
```

### `git pull`
**What it does**: Fetches and merges changes from remote repo to your local.
```bash
git pull origin main
```

### `git push`
**What it does**: Uploads your changes to a remote GitHub repo.
```bash
git push origin main
```

---

## 📦 PACKAGE MANAGEMENT (APT for Ubuntu/Debian)

### `sudo apt update`
**What it does**: Refreshes the list of available packages.
```bash
sudo apt update
```

### `sudo apt upgrade`
**What it does**: Installs the latest versions of all packages.
```bash
sudo apt upgrade
```

### `sudo apt install <package>`
**What it does**: Installs a software package.
```bash
sudo apt install git
```

---

## 🧠 BONUS: Shortcuts to Master

- `TAB` → Autocomplete filenames/folders
- `CTRL + C` → Cancel running command
- `CTRL + L` → Clear terminal (same as `clear`)
- `CTRL + D` → Exit shell
- `!!` → Run previous command again
- `!git` → Run the last command starting with "git"

---

## 💬 Example Git Workflow

```bash
git init
touch index.html
git add index.html
git commit -m "initial commit"
git remote add origin https://github.com/yourname/project.git
git push -u origin main
```

---

> 🚀 **RoeTechHub Rule**: Don’t just *run* commands. Understand their *intention*. Mastery beats memorization.

