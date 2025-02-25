# DevOps Lab 1
## Basic Git Commands
### Date: 7 January

## Objective
To understand and practice basic Git commands for version control.

## Basic Git Commands

### 1. Initialize a New Git Repository
To create a new local repository:
```sh
git init
```

### 2. Clone a Repository
Cloning a repository creates a local copy of a remote repository.
```sh
git clone <repository_url>
```
Example:
```sh
git clone https://github.com/user/repo.git
```

### 3. Check Repository Status
To check the current status of the repository:
```sh
git status
```

### 4. Add Files to Staging Area
To stage changes for commit:
```sh
git add <filename>
```
To add all changes:
```sh
git add .
```

### 5. Commit Changes
To save changes in the local repository:
```sh
git commit -m "Your commit message"
```

### 6. Set Up SSH for GitHub
To generate an SSH key:
```sh
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```
To add the SSH key to the SSH agent:
```sh
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```
To add the SSH key to your GitHub account:
1. Copy the SSH key:
   ```sh
   cat ~/.ssh/id_rsa.pub
   ```
2. Add it to GitHub under Settings > SSH and GPG keys.

### 7. Push Changes to Remote Repository
To upload local changes to a remote repository:
```sh
git push origin <branch_name>
```
Example:
```sh
git push origin main
```

## Conclusion
This lab introduced basic Git commands to manage version control. Further labs will cover branching, merging, and conflict resolution.

## Additional Resources
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com/en)

