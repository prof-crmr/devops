# GitLab Lab Exercise: Reverting Changes

## Objective
The objective of this Lab Exercise is to understand how to revert changes in Git using different commands: `git reset`, `git reset --hard`, and `git revert`. By following the steps and examples provided, you will gain a better understanding of when and how to use each command.

## Prerequisites
1. Basic understanding of Git concepts (e.g., repository, commit, branch).
2. Git installed on your local machine.
3. Familiarity with the command line or terminal.

## Steps

### Step 1: Cloning the Repository
1. Open your terminal or Git Bash.
2. Navigate to the directory where you want to clone the repository.
3. Run the following command to clone the repository to your local machine:

git clone <repository_url>

Replace `<repository_url>` with the URL of the repository you want to clone.

### Step 2: Making Changes
1. Navigate into the cloned repository using the terminal.
2. Modify a file or create a new file in the repository to simulate changes.
3. Run the following commands to stage and commit the changes:

git add .
git commit -m "Make changes for demonstration"

This creates a new commit with the changes.

### Step 3: Using `git reset`
1. Run the following command to view the commit history:

git log --oneline

Make a note of the commit hash (e.g., ABC123) of the commit you want to revert.
2. Run the following command to revert the changes using `git reset`:

git reset <commit_hash>

Replace `<commit_hash>` with the hash of the commit you want to revert.
- The default mode for `git reset` is "mixed," which unstages the changes and keeps the modifications in your working directory.
- You can also use `--soft` to keep the changes staged, or `--hard` to discard both the changes and the commit entirely.

### Step 4: Using `git reset --hard`
1. If you haven't already, run the following command to view the commit history:

git log --oneline

Make a note of the commit hash (e.g., DEF456) of the commit you want to revert.
2. Run the following command to revert the changes using `git reset --hard`:

git reset --hard <commit_hash>

Replace `<commit_hash>` with the hash of the commit you want to revert.
- The `--hard` option completely discards the changes and resets both the index and the working directory to the specified commit.

### Step 5: Using `git revert`
1. If you haven't already, run the following command to view the commit history:

git log --oneline

Make a note of the commit hash (e.g., GHI789) of the commit you want to revert.
2. Run the following command to revert the changes using `git revert`:

git revert <commit_hash>

Replace `<commit_hash>` with the hash of the commit you want to revert.
- `git revert` creates a new commit that undoes the changes made in the specified commit, effectively reverting the changes while preserving the commit history.

## Explanation

### `git reset`
- The `git reset` command allows you to move the branch pointer to a different commit, effectively resetting the state of the branch.
- By default, `git reset` is in "mixed" mode, which moves the branch pointer and updates the index to the specified commit, but keeps the changes in your working directory.
- You can use the `--soft` option to keep the changes staged or `--hard` option to discard both the changes and the commit entirely.

### `git reset --hard`
- The `git reset --hard` command is similar to `git reset` but discards both the changes and the commit entirely.
- It moves the branch pointer and updates the index and the working directory to the specified commit, effectively resetting the branch to the given commit.

### `git revert`
- The `git revert` command creates a new commit that undoes the changes made in a previous commit, effectively reverting the changes while preserving the commit history.
- It is a safer option when working on shared branches because it does not modify existing commits; instead, it adds new commits to reverse the changes.

By understanding the differences between `git reset`, `git reset --hard`, and `git revert`, you can choose the appropriate command for reverting changes based on your requirements and workflow.

Make sure to replace <repository_url> with the actual URL of the repository you want to clone, and <commit_hash> with the respective commit hashes in the respective steps. This Lab Exercise provides a step-by-step guide and explanations for each command to help you understand how to revert changes using git reset, git reset --hard, and git revert.
