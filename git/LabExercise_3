# Git Stash Lab Exercise: Managing Work in Progress

## Objective
The objective of this Lab Exercise is to provide training to your team on the usage of Git's stash feature for managing work in progress. By the end of this training, your team will be able to:

- Understand the purpose and benefits of using Git's stash feature.
- Know how to stash changes to save work in progress.
- Learn how to apply and manage stashed changes effectively.

## Prerequisites
1. Basic understanding of Git concepts (e.g., repository, commit, branch, stash).
2. Git installed on the team members' machines.

## Lab Exercise: Using Git Stash to Manage Work in Progress

Scenario:
Suppose your team is working on a web application called "AwesomeApp." You are currently working on implementing a new feature in a branch called `feature/new-feature`, but you need to switch to another branch to fix an urgent bug. Instead of committing your unfinished work, you can use Git's stash feature to temporarily store your changes and switch to the bug-fix branch. Once you are done with the bug fix, you can apply the stashed changes back to the `feature/new-feature` branch.

Step 1: Saving Work in Progress
1. Open your terminal or Git Bash.
2. Check the status of your working directory using `git status`. Ensure there are uncommitted changes that you want to stash.
3. Use the following command to stash your changes:

**git stash save "Work in progress: Feature implementation"**

This command saves your changes in a new stash with a descriptive message.

Step 2: Switching to the Bug-Fix Branch
1. Use `git branch` to list the available branches and verify that the bug-fix branch exists.
2. Switch to the bug-fix branch using the following command:

**git checkout bug-fix**

Now you can work on fixing the urgent bug without any conflicts with your feature implementation.

Step 3: Applying Stashed Changes
1. After fixing the bug, switch back to the `feature/new-feature` branch using `git checkout`.
2. Retrieve the stashed changes using the following command:

**git stash apply**

This command applies the most recent stash to your working directory. If you have multiple stashes, you can specify a stash by its index or name.
3. Use `git stash list` to see the list of available stashes and their details.

Step 4: Resolving Conflicts (If Any)
1. If there are any conflicts between the stashed changes and the current branch, you need to resolve them manually.
2. Open the conflicted files, edit them to resolve the conflicts, and save the changes.
3. Use `git add` to stage the resolved files.
4. Run `git stash drop` to remove the applied stash if you no longer need it.

Step 5: Completing the Feature Implementation
1. Continue working on the feature implementation, building upon the applied stashed changes.
2. Stage and commit your changes as usual once you have completed the feature implementation.

Congratulations! You have successfully completed the Lab Exercise, learning how to use Git's stash feature to manage work in progress. Stashing changes allows you to switch between branches and tasks without losing your unfinished work.

Refer to the [Git documentation on stash](https://git-scm.com/docs/git-stash) for more details on advanced options and additional use cases.


