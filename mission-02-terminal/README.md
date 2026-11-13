# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
The task was to use the Terminal to look around my folders, create and manage practice files safely, understand flags and pipes, and explain what a package manager does.

## 2. Work completed

### Task 2.1 — Basic Terminal operations

| Operation / command name | What it does | What I observed |
|--------------------------|--------------|-----------------|
| `pwd` (current-directory display) | Prints the full path of the folder I am in | It showed the path ending in my project folder, digital-detective-8480 |
| `ls` (directory listing) | Lists the files and folders in the current location | It listed the mission folders, evidence and README.md |
| `ls -l` (detailed listing) | Lists items with extra details like permissions, owner, size and date | Each item appeared on its own line with details |
| `cd` (change directory) | Moves me into another folder; `cd ..` moves to the parent folder | `cd mission-02-terminal` moved me into that folder and `cd ..` moved me back up |
| `mkdir` (create directory) | Creates a new folder | `terminal-practice` appeared inside mission-02-terminal |
| `touch` (create empty file) | Creates an empty file | `notes.txt` was created with nothing inside |
| `cp` (copy file) | Makes a copy of a file under a new name | `notes-copy.txt` appeared and `notes.txt` stayed |
| `mv` (move / rename file) | Moves a file or renames it | `notes-copy.txt` became `notes-renamed.txt` and the old name disappeared |
| `cat` (display file contents) | Prints what is inside a file | It printed the lines I had written in `notes.txt` |

### Task 2.2 — Practising file changes safely
Inside `mission-02-terminal/terminal-practice` I created `notes.txt`, wrote one line with `echo "..." > notes.txt`, and added a second line with `echo "..." >> notes.txt`. `cat notes.txt` showed both lines. I then made a backup copy with `cp` and renamed it with `mv`.

Answers:
- **Replacing vs adding to the end:** `>` replaces everything in a file with the new text, so the old content is lost. `>>` keeps the old content and adds the new text at the end.
- **Copying vs moving:** copying makes a second file and the original stays where it is. Moving takes the file from one place or name to another, so the original name no longer exists.
- **What the current-directory display gives:** `pwd` shows the full path of the folder I am in, so I know exactly where my commands will act.
- **Why a directory listing is useful:** `ls` lets me see which files and folders are there, so I can check that something was created, copied or renamed.

### Task 2.3 — Flags and pipes
- `ls` showed only the names of the visible files and folders.
- `ls -lah` showed more: `-l` gives a detailed list (permissions, owner, size, date), `-a` includes hidden files (names starting with a dot, such as `.git`), and `-h` shows sizes in a readable form like KB instead of raw bytes.
- A flag (option) changes how a command behaves without changing the command itself.

For the pipe, I ran `ls -lah | head -5`. The pipe symbol `|` takes the output of the command on its left and sends it as input to the command on its right. Here, `ls -lah` produces the full detailed listing, and `head -5` shows only the first five lines of it. A pipe lets me combine small commands to do something bigger.

### Task 2.4 — Package managers
Homebrew is installed on my Mac. `brew --version` showed its version number and `brew list` showed the packages it manages, such as git and python. I did not install or uninstall anything.
A package manager is a tool that installs, updates and removes software from one place using simple commands. This is useful because it saves me from downloading installers by hand, it can install the other software a program depends on, and it keeps everything easier to update and remove.

## 3. Commands / tools used
- `pwd`: shows the current folder path.
- `ls`, `ls -l`, `ls -lah`: list files and folders, with more detail or hidden files when flags are added.
- `cd`: changes the current folder.
- `mkdir`: creates a folder.
- `touch`: creates an empty file.
- `cp`: copies a file.
- `mv`: moves or renames a file.
- `echo` with `>` and `>>`: writes text to a file, replacing or appending.
- `cat`: displays a file's contents.
- `head`: shows only the first lines of its input.
- `|` (pipe): sends one command's output into another command.
- `brew --version` and `brew list`: check Homebrew and its packages.
- Git: `git add`, `git commit`, `git push` to save the mission.

## 4. My understanding
The Terminal lets me control the computer by typing commands. I learned that `pwd` and `ls` help me know where I am and what is there, `cd` moves me around, and `mkdir`, `touch`, `cp` and `mv` create and manage files. The difference between `>` and `>>` is important because one can erase existing content. Flags change how commands behave, and pipes connect commands so one command's output becomes the next one's input. Package managers make installing and updating software easier and safer.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-02-terminal/README.md`
- `mission-02-terminal/terminal-practice/notes.txt`
- `mission-02-terminal/terminal-practice/notes-renamed.txt`
- `mission-02-terminal/terminal-practice/notes-backup-renamed.txt`

No screenshots were added, because Terminal output shows my computer username.

## 8. Commit details
Commit message: "Complete Terminal and file management mission"

The work was pushed to GitHub and I confirmed the files and commit are visible.