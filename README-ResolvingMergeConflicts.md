# Resolving Merge Conflicts

Despite best efforts, merge conflicts can still happen. Here’s how to resolve them:

## Detecting a Conflict

When you attempt to merge branches, Git will automatically detect conflicts. You’ll see something like this:

```bash
Auto-merging file.txt
CONFLICT (content): Merge conflict in file.txt
Automatic merge failed; fix conflicts and then commit the result.
```

## Resolving a Conflict

1. **Open the Conflicted File:** Locate the conflict markers in the file.
    ```text
    <<<<<<< HEAD
    Code from your branch
    =======
    Code from the branch you're merging
    >>>>>>> other-branch
    ```
2. **Resolve the Conflict:** Edit the file to keep the desired changes and remove the conflict markers.
3. **Stage the Resolved File:**
    ```bash
    git add file.txt
    ```
4. **Complete the Merge:** Finalize the merge by committing the changes.
    ```bash
    git commit
    ```

## Test Thoroughly

After resolving conflicts, ensure the code works as expected by running tests and reviewing the changes.

## Final Tips

- If a conflict is too complex, consider discussing the resolution with your team.
- Use Git tools like `git mergetool` to assist in resolving conflicts.
