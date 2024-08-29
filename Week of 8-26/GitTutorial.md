# Git Tutorial

In this tutorial, we will learn how to clone, add, commit, and push to a GitHub repository.

## Cloning a Repository

To clone a repository, follow these steps:

1. Open your terminal or command prompt.
2. Navigate to the directory where you want to clone the repository. Example: 'cd Desktop'
3. Use the `git clone` command followed by the repository URL. For example:
    ```
    git clone https://github.com/username/repository.git
    ```
    Replace the link with either the HTTPS or SSH link from GitHub.

## Adding and Committing Changes

At this point, you should have modified your code and are now planning to push to github. You will do all of the following within the VS code terminal.

To add and commit changes, follow these steps:

1. Use the `git add` command to stage the changes.
    ```
    git add .
    ```
    The '.' signifies all files that are in the directory.
2. Use the `git commit` command to commit the changes with a descriptive message. For example:
    ```
    git commit -m "Added new feature"
    ```

## Pushing Changes to GitHub

To push your changes to a GitHub repository, follow these steps:

1. Use the `git push` command. For example:
    ```
    git push
    ```
Repeat all steps necessary when doing future commits and pushes.

End of tutorial.
