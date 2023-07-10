# GitLab Lab Exercise: Git Tagging Concepts

## Objective
The objective of this Lab Exercise is to understand Git tagging concepts, including creating tags, listing tags, and using annotated tags and lightweight tags. By following the steps and examples provided, you will gain a better understanding of how to use Git tags for marking important milestones or releases in your repository.

## Prerequisites
1. Basic understanding of Git concepts (e.g., repository, commit).
2. Git installed on your local machine.
3. Familiarity with the command line or terminal.

## Steps

### Step 1: Cloning the Repository
1. Open your terminal or Git Bash.
2. Navigate to the directory where you want to clone the repository.
3. Run the following command to clone the repository to your local machine:

git clone <repository_url>

Replace `<repository_url>` with the URL of the repository you want to clone.

### Step 2: Creating a Tag
1. Navigate into the cloned repository using the terminal.
2. Run the following command to view the commit history:

git log --oneline

Make a note of the commit hash (e.g., ABC123) of the commit you want to tag.
3. Run the following command to create an annotated tag:

git tag -a <tag_name> <commit_hash> -m "<tag_message>"

Replace `<tag_name>` with the desired name for your tag, `<commit_hash>` with the commit hash you want to tag, and `<tag_message>` with a descriptive message for the tag.
- Annotated tags include additional metadata, such as the author, date, and message.

### Step 3: Listing Tags
1. Run the following command to list all the tags in the repository:

git tag

This command displays a list of tags in alphabetical order.
2. To view the details of an annotated tag, run the following command:

git show <tag_name>

Replace `<tag_name>` with the name of the tag you want to view.
- This command shows the commit information and the tag message associated with the specified tag.

### Step 4: Checking out a Tag
1. Run the following command to check out a specific tag:

git checkout <tag_name>

Replace `<tag_name>` with the name of the tag you want to check out.
- Checking out a tag puts your repository in a "detached HEAD" state, meaning you are not on any branch but at the specific commit associated with the tag.
- You can view and work with the code at the state of the tagged commit.

### Step 5: Creating Lightweight Tags
1. Navigate into the cloned repository using the terminal.
2. Run the following command to create a lightweight tag:

git tag <tag_name> <commit_hash>

Replace `<tag_name>` with the desired name for your tag, and `<commit_hash>` with the commit hash you want to tag.
- Lightweight tags are just references to specific commits and do not include additional metadata.

## Explanation

### Tags in Git
- Tags in Git are used to mark important milestones or releases in a repository.
- Annotated tags include additional metadata, such as the author, date, and message, and are typically used for releases or major versions.
- Lightweight tags are just references to specific commits and are often used for marking specific points or versions.

### Creating Tags
- To create an annotated tag, you use the `git tag -a` command followed by the tag name, the commit hash, and a message.
- For example: `git tag -a v1.0.0 ABC123 -m "Release version 1.0.0"`
- To create a lightweight tag, you simply use the `git tag` command followed by the tag name and the commit hash.
- For example: `git tag v1.0.0 ABC123`

### Listing Tags
- You can list all the tags in a repository using the `git tag` command.
- To view the details of an annotated tag, you can use the `git show` command followed by the tag name.
- For example: `git show v1.0.0`

### Checking out Tags
- You can check out a specific tag using the `git checkout` command followed by the tag name.
- For example: `git checkout v1.0.0`
- Checking out a tag puts your repository in a "detached HEAD" state, allowing you to view and work with the code at the state of the tagged commit.

By understanding Git tagging concepts and using the provided examples, you can mark important milestones or releases in your repository and easily navigate to specific points in your commit history.

Make sure to replace <repository_url> with the actual URL of the repository you want to clone, <tag_name> with the desired tag names, and <commit_hash> with the respective commit hashes in the respective steps. This Lab Exercise provides a step-by-step guide and explanations for creating tags, listing tags, checking out tags, and understanding the difference between annotated tags and lightweight tags in Git.

