# 💻 Git Basics: Your Hands-On CLI Lesson

This lesson uses **Git Bash** (installed with Git on Windows) to teach the absolute basics of saving and restoring your code.

---

## What is Git For? (Saving and Undoing)

Git is a **Version Control System**. It allows you to take **snapshots** (called **commits**) of your project's files. This acts like a **time machine** for your code, letting you easily go back to a working version if you make a mistake later.

---

## Lesson 1: Starting Your Project

### 1. Open Git Bash

* Find and open **Git Bash** from your Windows Start menu.

### 2. Create and Enter Project Folder

* Type the following commands:
    ```bash
    mkdir my-first-code
    cd my-first-code
    ```

### 3. Initialize Git

Tells Git to start tracking this folder.

| Command | Purpose |
| :--- | :--- |
| `git init` | **Initializes** Git. (Do this **once** per project.) |

**In Git Bash:**

```bash
git init
````

-----

## Lesson 2: Saving Your First Snapshot

### 1\. Create and Change Files

  * In your file explorer, navigate to the `my-first-code` folder.
  * Create a file named **`hello.txt`** and add some content. Save the file.

### 2\. Check Status

See what files Git has noticed but isn't tracking yet.

| Command | Purpose |
| :--- | :--- |
| `git status` | Shows which files are **untracked** (new/red) or **modified**. |

**In Git Bash:**

```bash
git status
```

### 3\. Stage the File

You must prepare the files you want to save. This moves them to the **Staging Area**.

| Command | Purpose |
| :--- | :--- |
| `git add .` | Stages **ALL** new and modified files, preparing them for the snapshot. |

**In Git Bash:**

```bash
git add .
```

### 4\. Take the Snapshot (Commit)

This is the final save command, making the snapshot permanent.

| Command | Purpose |
| :--- | :--- |
| `git commit -m "Message"` | Saves the staged files. Your message explains what you accomplished. |

**In Git Bash:**

```bash
git commit -m "Initial working version of hello file"
```

-----

## Lesson 3: Viewing and Undoing Mistakes

### 1\. View History

Look at the list of all your permanent saves.

| Command | Purpose |
| :--- | :--- |
| `git log` | Displays a list of all snapshots (commits) and their unique **Commit IDs**. |

**In Git Bash:**

```bash
git log
```

### 2\. Revert the Mistake

If you made a bad change and saved it, you can undo it by reverting the *mistake* snapshot.

1.  Use **`git log`** to find and copy the **Commit ID** of the **MISTAKE** snapshot you want to undo.
2.  Run the revert command:

| Command | Purpose |
| :--- | :--- |
| `git revert <Commit ID>` | Creates a **new safe commit** that undoes the changes of the specified mistake snapshot, restoring your code. |

**In Git Bash:**

```bash
# Example: Replace the ID with the actual ID of the bad commit
git revert a1b2c3d4e5f67890... 
```

*(Git will open an editor to confirm the message. Save and close the editor to complete the revert.)*

