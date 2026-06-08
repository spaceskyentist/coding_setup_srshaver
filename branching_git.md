# How to Create a New GitHub Branch in VS Code and Merge It Back into Main

## 1. Open the Repository in VS Code

Open VS Code and open the folder containing your GitHub repository.

Verify that you are currently on the `main` branch. The active branch is displayed in the bottom-left corner of VS Code.

---

## 2. Pull the Latest Changes from Main

Before creating a new branch, make sure your local copy of `main` is up to date.

### Using VS Code

1. Open the **Source Control** panel.
2. Click the **...** menu.
3. Select **Pull**.

### Using the Terminal

```bash
git checkout main
git pull origin main
```

---

## 3. Create a New Branch

### Using VS Code

1. Click the branch name in the bottom-left corner.
2. Select **Create New Branch**.
3. Enter a descriptive branch name, for example:

```text
add-new-roi-files
```

4. Press Enter.

VS Code will automatically switch to the new branch.

### Using the Terminal

```bash
git checkout -b add-new-roi-files
```

---

## 4. Make Your Changes

Edit, add, or delete files as needed.

You can view modified files in the **Source Control** panel.

---

## 5. Stage and Commit Your Changes

### Using VS Code

1. Open the **Source Control** panel.
2. Click the **+** icon next to each file to stage changes, or stage all changes at once.
3. Enter a commit message.
4. Click **Commit**.

### Using the Terminal

```bash
git add .
git commit -m "Add new ROI files"
```

---

## 6. Push the Branch to GitHub

### Using VS Code

Click **Publish Branch** or **Sync Changes**.

### Using the Terminal

```bash
git push -u origin add-new-roi-files
```

The `-u` flag sets the upstream branch so future pushes only require:

```bash
git push
```

---

## 7. Switch Back to Main

### Using VS Code

1. Click the branch name in the bottom-left corner.
2. Select `main`.

### Using the Terminal

```bash
git checkout main
```

---

## 8. Pull the Latest Version of Main

Before merging, update your local `main` branch.

```bash
git pull origin main
```

---

## 9. Merge Your Branch into Main

### Using VS Code

1. Confirm you are currently on `main`.
2. Open the Command Palette:

   - Windows/Linux: `Ctrl + Shift + P`
   - macOS: `Cmd + Shift + P`

3. Search for:

```text
Git: Merge Branch
```

4. Select your branch (e.g., `add-new-roi-files`).

### Using the Terminal

```bash
git merge add-new-roi-files
```

---

## 10. Resolve Merge Conflicts (If Necessary)

If conflicts occur:

1. Open each conflicted file.
2. Review the conflicting sections.
3. Choose which changes to keep.
4. Save the file.
5. Stage the resolved files.

### Complete the Merge

```bash
git add .
git commit
```

---

## 11. Push the Updated Main Branch

After the merge is complete, push the updated `main` branch to GitHub.

```bash
git push origin main
```

---

## 12. (Optional) Delete the Branch

After the branch has been successfully merged, it can be removed.

### Delete the Local Branch

```bash
git branch -d add-new-roi-files
```

### Delete the Remote Branch

```bash
git push origin --delete add-new-roi-files
```

---

# Quick Reference Workflow

```bash
git checkout main
git pull origin main

git checkout -b my-new-branch

# Make changes

git add .
git commit -m "Describe changes"

git push -u origin my-new-branch

git checkout main
git pull origin main

git merge my-new-branch

git push origin main
```

## Best Practices

- Always start from an up-to-date `main` branch.
- Use descriptive branch names.
- Commit small, logical changes.
- Pull the latest `main` before merging.
- Resolve conflicts carefully before pushing.
- Delete merged branches to keep the repository clean.
