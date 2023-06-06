# Git Cheat Sheet

Git is a distributed version control system that allows developers to track changes, collaborate on projects, and manage source code efficiently. This cheat sheet provides an overview of all the essential Git commands to help developers navigate their repositories effectively.

## Table of Contents
1. [Configuration](#configuration)
2. [Repository Creation](#repository-creation)
3. [Cloning Repositories](#cloning-repositories)
4. [Basic Workflow](#basic-workflow)
5. [Branching and Merging](#branching-and-merging)
6. [Remote Repositories](#remote-repositories)
7. [Collaborative Workflows](#collaborative-workflows)
8. [Stashing Changes](#stashing-changes)
9. [Inspecting and Comparing](#inspecting-and-comparing)
10. [Undoing Changes](#undoing-changes)
11. [Gitignore](#gitignore)

## Configuration
- Set up your name: `git config --global user.name "Your Name"`
- Set up your email: `git config --global user.email "youremail@example.com"`
- Configure default text editor: `git config --global core.editor "editor_name"`

## Repository Creation
- Initialize a new repository: `git init`
- Clone an existing repository: `git clone <repository_url>`
- Initialize a new repository with a README: `git init <directory_name> --initial-branch=<branch_name>`
- Clone a repository to a specific directory: `git clone <repository_url> <directory_name>`

## Cloning Repositories
- Clone a repository: `git clone <repository_url>`
- Clone a repository to a specific directory: `git clone <repository_url> <directory_name>`

## Basic Workflow
- Check repository status: `git status`
- Stage changes for commit: `git add <file_name>` (or use `.` to stage all changes)
- Unstage changes: `git restore --staged <file_name>`
- Commit changes: `git commit -m "Commit message"`
- Amend the last commit: `git commit --amend`
- Push changes to remote repository: `git push origin <branch_name>`
- Pull changes from remote repository: `git pull origin <branch_name>`
- Fetch changes from remote repository: `git fetch origin`

## Branching and Merging
- Create a new branch: `git branch <branch_name>`
- Switch to a branch: `git checkout <branch_name>`
- Create and switch to a new branch: `git checkout -b <branch_name>`
- List all branches: `git branch`
- Delete a branch: `git branch -d <branch_name>`
- Merge branches: `git merge <branch_name>`
- Resolve merge conflicts: Open conflicted files, manually resolve conflicts, and commit changes.

## Remote Repositories
- Add a remote repository: `git remote add <remote_name> <remote_url>`
- List remote repositories: `git remote -v`
- Remove a remote repository: `git remote remove <remote_name>`

## Collaborative Workflows
- Push a branch to a remote repository: `git push origin <branch_name>`
- Create a pull request (PR) on GitHub/Bitbucket
- Review and merge PR on GitHub/Bitbucket

## Stashing Changes
- Stash changes: `git stash`
- List stashed changes: `git stash list`
- Apply stashed changes: `git stash apply <stash_id>`
- Clear all stashed changes: `git stash clear`

## Inspecting and Comparing
- View commit history: `git log`
- View file changes: `git diff`
- View changes between commits: `git diff <commit_hash1> <commit_hash2>`
- View branches' commit history: `git log --graph --oneline --decorate --all`

## Undoing Changes
- Undo the last commit, keeping changes: `git reset HEAD~1`
- Discard changes in a file: `git checkout -- <file_name>`
- Revert a commit: `git revert <commit_hash>`

## Gitignore
- Create a .gitignore file: `touch .gitignore`
- Specify files and directories to ignore in the .gitignore file
- Use patterns and wildcards to match files/directories

Feel free to use this cheat sheet as a quick reference guide for your Git workflows. Happy coding!

