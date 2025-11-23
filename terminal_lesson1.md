
## 💻 Git Bash Terminal Cheat Sheet

| Command | Category | Purpose | Example |
| :--- | :--- | :--- | :--- |
| `ls` | **Viewing** | **L**i**s**t the files and folders in the current directory. | `ls -a` (shows hidden files) |
| `pwd` | **Viewing** | **P**rint **W**orking **D**irectory. Shows the full path of the folder you are currently in. | `pwd` |
| `cd <folder>` | **Navigation** | **C**hange **D**irectory. Moves you into a specified folder. | `cd Documents` |
| `cd ..` | **Navigation** | Moves you up **one level** (to the parent folder). | `cd ..` |
| `cd ~` | **Navigation** | Moves you back to your **Home** directory (your user folder). | `cd ~` |
| `mkdir <name>` | **File Mgmt** | **M**a**k**e **Dir**ectory. Creates a new, empty folder. | `mkdir my-project` |
| `touch <file>` | **File Mgmt** | Creates a new, empty file. | `touch notes.txt` |
| `rm <file>` | **File Mgmt** | **R**e**m**oves (deletes) a specific file. | `rm old_file.txt` |
| `rm -r <folder>` | **File Mgmt** | **R**emoves a folder and all its contents (`-r` is recursive). (Use carefully\!) | `rm -r temp_data` |
| `clear` | **Utility** | Clears the previous commands and output from the screen. | `clear` |

-----

## ⚠️ A Critical Safety Note: Avoid `rm -f`

The command **`rm -f`** adds the **f**orce flag (`-f`).

  * **What it does:** It tells the system to delete the file immediately and **do not ask for confirmation.**
  * **Why to avoid it:** When you run the standard `rm <file>`, the system sometimes asks for a confirmation or stops you if the file is protected. Using `rm -f` bypasses these safety checks. For a beginner, typing this command incorrectly can instantly delete important, unsaved files or even critical system files without any warning. **Only use this flag if you are an experienced user and absolutely certain of what you are deleting.**

-----

## 📝 Practice Scenarios (Using Git Bash)

Let's integrate the file deletion into the workflow:

1.  **Go to Documents:** Move into the **Documents** folder:
    ```bash
    cd Documents
    ```
2.  **Create Project Folder:** Make a new folder named `website-project`:
    ```bash
    mkdir website-project
    ```
3.  **Enter Project Folder:** Move into the new folder:
    ```bash
    cd website-project
    ```
4.  **Create Starting File:** Create an empty file called `index.html`:
    ```bash
    touch index.html
    ```
5.  **Create Temp File:** Create a file you want to delete later:
    ```bash
    touch temp_notes.txt
    ```
6.  **Delete Temp File:** Use `rm` to safely delete the temporary file:
    ```bash
    rm temp_notes.txt
    ```
7.  **Verify:** Use `ls` to check that only `index.html` remains.
    ```bash
    ls
    ```

You're now ready to start the Git tracking process with your clean `website-project` folder\!
