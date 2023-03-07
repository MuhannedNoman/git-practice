# Small activity to practice git

## First part
1. Install Git on your computer: The first step is to download and install Git on your computer. You can find the installation instructions on the [official Git website](https://git-scm.com/downloads).

2. Create a new Git repository: Open a new terminal or command prompt window, navigate to the folder where you want to create a new Git repository, and type the following command:

```
git init
``` 
This command creates a new Git repository in the current directory.

3. Create a new file: Use your text editor or IDE to create a new file in the repository folder. Add some text to the file.

4. Add the file to the staging area: Use the following command to add the file to the Git staging area:

```
git add <filename>
```
Replace <filename> with the name of the file you just created.

5. Commit the changes: Use the following command to commit the changes to the repository:
```
git commit -m "Initial commit"
```
The -m option allows you to add a commit message describing the changes you made.

6. Make some changes: Open the file you just created and make some changes to the text. Save the changes.

7. Check the status: Use the following command to check the status of your repository:

```
git status
```
This command shows you which files have been changed since the last commit.

8. Add the changes to the staging area: Use the following command to add the changes to the staging area:
```
git add <filename>
```
Replace <filename> with the name of the file you just edited.

9. Commit the changes: Use the following command to commit the changes to the repository:
```
git commit -m "Made some changes"
```
10. View the commit history: Use the following command to view the commit history of your repository:
```
git log
```
This command shows you a list of all the commits you've made to the repository, including the commit message and the date and time of the commit.
## Second part
11. Create a new branch: Use the following command to create a new branch:
```
git branch <branch-name>
```
Replace `<branch-name>` with the name of the new branch you want to create. For example:

```
git branch feature-branch
```
This command creates a new branch called `feature-branch` that is based on the current branch.

12. Switch to the new branch: Use the following command to switch to the new branch:
```
git checkout <branch-name>
```
For example:

```
git checkout feature-branch
```
This command switches your working directory to the new branch.

13. Make some changes: Open the file you created earlier and make some additional changes to the text. Save the changes.

14. Add the changes to the staging area: Use the following command to add the changes to the staging area:

```
git add <filename>
```
Replace `<filename>` with the name of the file you just edited.

15. Commit the changes: Use the following command to commit the changes to the repository:
```
git commit -m "Added some features"
```
Switch back to the main branch: Use the following command to switch back to the main branch:
```
git checkout main
```
Merge the feature branch: Use the following command to merge the feature branch into the main branch:
```
git merge <branch-name>
```
Replace `<branch-name>` with the name of the feature branch you want to merge. For example:

```
git merge feature-branch
```
This command combines the changes you made in the feature branch with the changes in the main branch.
## Third part
Create a new branch: Use the following command to create a new branch:
```
git branch <branch-name>
```
Replace `<branch-name>` with the name of the new branch you want to create. For example:

```
git branch conflict-branch
```
Switch to the new branch: Use the following command to switch to the new branch:
```
git checkout <branch-name>
```
For example:

```
git checkout conflict-branch
```
Make some changes: Open the file you created earlier and make some additional changes to the text. Save the changes.

Add the changes to the staging area: Use the following command to add the changes to the staging area:

```
git add <filename>
```
Replace `<filename>` with the name of the file you just edited.

Commit the changes: Use the following command to commit the changes to the repository:
```
git commit -m "Added some features"
```
Switch back to the main branch: Use the following command to switch back to the main branch:
```
git checkout main
```
Make some changes to the same file: Open the same file you edited earlier and make some additional changes to the text, but this time make sure the changes conflict with the changes you made in the feature branch. Save the changes.

Add the changes to the staging area: Use the following command to add the changes to the staging area:

```
git add <filename>
```
Replace `<filename>` with the name of the file you just edited.

Commit the changes: Use the following command to commit the changes to the repository:
```
git commit -m "Made some changes to the same file"
```
Merge the feature branch: Use the following command to merge the feature branch into the main branch:
```
git merge <branch-name>
```
Replace `<branch-name>` with the name of the feature branch you want to merge. For example:

```
git merge conflict-branch
```
Resolve conflicts: Git will detect the conflict and prompt you to resolve it. Open the file in question and you will see the conflicting changes marked with `<<<<<<< HEAD` and `>>>>>>> <branch-name>`. Edit the file to choose which changes to keep and delete the markers. For example:
```bash
This is the original text.

<<<<<<< HEAD
This is the conflicting change from the main branch.
=======
This is the conflicting change from the feature branch.
>>>>>>> conflict-branch

This is the additional text.
```
In this example, we want to keep the change from the feature branch, so we delete the lines containing `<<<<<<< HEAD` and `=======`, and keep the lines containing `This is the conflicting change from the feature branch.`

Add the resolved changes to the staging area: Use the following command to add the resolved changes to the staging area:
```
git add <filename>
```
Commit the changes: Use the following command to commit the resolved changes to the repository:
```
git commit -m "Resolved conflicts"
```
