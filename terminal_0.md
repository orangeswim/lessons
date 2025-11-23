
## 🧭 Your First Terminal Lesson: Folder Navigation

The most important thing to learn before using Git is how to move around your computer's folders (called **directories** in the command line) using **Git Bash**.

### 1. The Core Commands

You only need to master two commands to move around: **`pwd`** (Where Am I?) and **`cd`** (Go Somewhere).

| Command | Purpose | Analogy |
| :--- | :--- | :--- |
| **`pwd`** | **P**rint **W**orking **D**irectory. Shows the full path of the folder you are currently inside. | **"Where am I right now?"** |
| **`ls`** | **L**i**s**t. Shows all files and sub-folders within your current directory. | **"What doors can I walk through?"** |
| **`cd <name>`** | **C**hange **D**irectory. Moves you into a specified folder. | **"Go into the Living Room."** |
| **`cd ..`** | Change Directory Up. Moves you up **one level** to the parent folder. | **"Go back out to the Hallway."** |
| **`mkdir <name>`** | **M**a**k**e **Dir**ectory. Creates a new, empty folder. | **"Build a new closet."** |

---

## 2. 📝 Hands-On Practice: Creating and Moving

Open **Git Bash** from your Windows Start menu and try these steps. Remember to use the **Tab key** for auto-completion to avoid typing out full names!

| Action | Command | Your Location (Directory) |
| :--- | :--- | :--- |
| **A. Start (Go Home)** | `cd ~` | `/c/Users/YourName` (Your main folder) |
| **B. Create a Folder** | `mkdir MyCodeProjects` | (Stays in Home) |
| **C. Move Down (Into Projects)** | `cd MyCodeProjects` | `/c/Users/YourName/MyCodeProjects` |
| **D. Create a Sub-Folder** | `mkdir FirstWebsite` | (Stays in MyCodeProjects) |
| **E. Move Down Again** | `cd FirstWebsite` | **/c/Users/YourName/MyCodeProjects/FirstWebsite** |
| **F. Move Up One Level** | `cd ..` | `/c/Users/YourName/MyCodeProjects` |
| **G. Move Up Two Levels** | `cd ../..` | `/c/Users/YourName` |
| **H. Verify Location** | `pwd` | Should show your Home folder path. |

---

## 3. 🧠 Advanced Navigation: Jumping Sideways

You can move out of one folder and into a different folder at the same level using one command.

Assume you are in the **`FirstWebsite`** folder and you want to jump into another folder named **`SecondApp`** that you created next to it.

1.  **Go Up One Level** (`..`)
2.  **Go Into the New Folder** (`/SecondApp`)

| Action | Command | Resulting Location |
| :--- | :--- | :--- |
| **Current Location** | `pwd` | `/c/Users/YourName/MyCodeProjects/FirstWebsite` |
| **Move Sideways** | `cd ../SecondApp` | `/c/Users/YourName/MyCodeProjects/SecondApp` |

---

Are you ready to move on to the **Terminal Cheat Sheet**, including how to delete files, or are you ready for the Git lesson itself?
