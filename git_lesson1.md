# 💾 Git: Your Code's Time Machine

Git is a tool that acts like a **save button with history** for your code. It lets you take **snapshots** (called commits) of your project, so if you break something later, you can easily go back to a working version.

---

## What is Git For? (Saving and Undoing)

Git is a **Version Control System**. Think of it as a personal safety net for your files:

1.  **Save Your Work (Commits):** Every time you finish a feature or make a set of changes you are happy with, you tell Git to take a permanent snapshot.
2.  **Go Back in Time (Reverting):** If you make changes that completely mess up your code, Git lets you easily throw away the bad code and restore a previous, good snapshot.

---

## 🛠️ The 3-Step Local Saving Workflow

To save your work, you move files through three main areas:

| Area | Purpose |
| :--- | :--- |
| **1. Working Directory** | Where you currently edit your files. |
| **2. Staging Area** | A waiting area where you select *exactly* which files will be in the next snapshot. |
| **3. Local Repository** | Where the permanent snapshots (commits) are saved. |

### The Essential Commands

| Command | Action | Description |
| :--- | :--- | :--- |
| **1. Start Tracking** | `git init` | Tells Git to start tracking your current folder. **(Do this once per project)**. |
| **2. Check What Changed**| `git status` | Shows you which files you have created or edited since your last save. |
| **3. Prepare the Save** | `git add .` | Selects ALL new and edited files and prepares them for the snapshot (**Staging**). |
| **4. Take the Snapshot** | `git commit -m "Your description"` | Takes the snapshot (saves it permanently). The description explains **what** you saved. |
| **5. View History** | `git log` | Shows a list of all your past saves (snapshots). |

---

## ↩️ How to Undo a Mistake (The "Oops!" Command)

This command is how you go back to a previous save.

1.  Use `git log` to find the ID of the good snapshot you want to return to. (It's a long string of numbers and letters, like `a1b2c3d4e5f6...`).
2.  Run the revert command:

| Command | Action | Description |
| :--- | :--- | :--- |
| **Revert** | `git revert <Commit ID>` | Creates a *new* snapshot that undoes all the changes made in the mistake snapshot. (This is the safest way to undo.) |
