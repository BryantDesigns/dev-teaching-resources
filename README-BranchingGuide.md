# How to Use Branches Effectively

To make the most of branching, follow these guidelines:

## Creating a Branch

1. **Checkout Main:** Start from the latest version of the main branch.
    ```bash
    git checkout main
    git pull origin main
    ```
2. **Create a New Branch:**
    ```bash
    git checkout -b feature/new-feature
    ```

## Working on a Branch

1. **Make Changes:** Develop your feature or fix.
2. **Commit Changes:** Regularly commit your work to the branch.
    ```bash
    git add .
    git commit -m "Add new feature"
    ```

## Keeping Your Branch Updated

1. **Pull Latest Changes from Main:**
    ```bash
    git fetch origin
    git merge origin/main
    ```
2. **Resolve Conflicts (if any):** Handle any merge conflicts before pushing your branch.

## Merging Back to Main

1. **Create a Pull Request:** When your feature is ready, create a pull request to merge your branch into the main branch.
2. **Code Review:** Ensure your code is reviewed by peers.
3. **Merge and Delete Branch:** After approval, merge your branch and delete it to keep the repository clean.
    ```bash
    git branch -d feature/new-feature
    ```
