# GitLab Lab Exercise: Difference Between `git pull` and `git fetch`

## Objective
The objective of this Lab Exercise is to understand the difference between the `git pull` and `git fetch` commands in Git. By following the steps and examples provided, you will gain a better understanding of when to use each command and how they differ in their behavior.

## Prerequisites
1. Basic understanding of Git concepts (e.g., repository, commit, branch, remote).
2. Git installed on your local machine.
3. Familiarity with the command line or terminal.

## Steps

### Step 1: Cloning the Repository
1. Open your terminal or Git Bash.
2. Navigate to the directory where you want to clone the repository.
3. Run the following command to clone the repository to your local machine:

**git clone <repository_url>**

Replace `<repository_url>` with the URL of the repository you want to clone.

### Step 2: Understanding `git pull`
1. Navigate into the cloned repository using the terminal.
2. Run the following command to view the remote branches:

**git branch -r**

This command lists the remote branches available in the repository.
3. Choose a remote branch to demonstrate the `git pull` command. Let's assume the chosen branch is `origin/main` (replace with your desired branch name).
4. Run the following command to switch to the chosen branch:

**git checkout <branch_name>**

Replace `<branch_name>` with the name of the chosen branch.
5. Make a note of the current commit (e.g., commit A) of the chosen branch.
6. Modify a file or create a new file in the repository.
7. Run the following commands to stage and commit the changes:

**git add .**

**git commit -m "Modify file(s) or create new file"**

This simulates a change made to the local branch.
8. Run the following command to push the changes to the remote repository:

**git push origin <branch_name>**

Replace `<branch_name>` with the name of the chosen branch.
9. Switch to a different branch (e.g., `main`) using the following command:

git checkout <other_branch>

Replace `<other_branch>` with the name of the other branch.
10. Run the following command to demonstrate `git pull`:
 ```
 git pull origin <branch_name>
 ```
 Replace `<branch_name>` with the name of the chosen branch.
11. Observe that the changes made in the chosen branch are pulled and merged into the current branch (e.g., `main`).

### Step 3: Understanding `git fetch`
1. Navigate into the cloned repository using the terminal.
2. Run the following command to demonstrate `git fetch`:

**git fetch origin**

This command fetches all the remote branches and their respective commits to your local repository.
3. Run the following command to view the remote branches and their associated commits:

**git branch -r**

This command lists the remote branches available in the repository, including their commits.
4. Choose a remote branch to merge into the current branch.
5. Run the following command to switch to the chosen branch:

**git checkout <branch_name>**

Replace `<branch_name>` with the name of the chosen branch.
6. Observe that the current branch now points to the latest commit of the chosen remote branch.
7. If desired, merge the chosen branch into the current branch using the following command:

**git merge origin/<branch_name>**

Replace `<branch_name>` with the name of the chosen branch.

## Explanation

### `git pull`
- The `git pull` command fetches the changes from the remote repository and merges them into the current branch in one step.
- It automatically performs a `git fetch` followed by a `git merge` to update the local branch with the remote changes.
- It's a convenient way to fetch and merge changes from the remote repository into the current branch.

### `git fetch`
- The `git fetch` command retrieves the latest changes from the remote repository but does not merge them into the current branch.
- It updates the remote tracking branches (e.g., `origin/main`) to reflect the latest state of the remote repository.
- It allows you to see the changes made in the remote repository without modifying your current branch.
- You can compare the fetched changes with your local branch, perform any necessary reviews or tests, and then merge them manually using the `git merge` command.

By understanding the difference between `git pull` and `git fetch`, you can choose the appropriate command based on your workflow and requirements. `git pull` is useful when you want to quickly update your local branch with the latest changes from the remote repository, while `git fetch` allows you to inspect the changes before merging them into your branch manually.


