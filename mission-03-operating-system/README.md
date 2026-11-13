# Mission 3 — Understand the operating system

## 1. Task / objective
The task was to explore my operating system with Terminal commands, look at running processes, understand paths and file permissions, and explain what an operating system is responsible for.

## 2. Work completed

### Task 3.1 — Explore my operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
|----------------------|-------------------|---------------------------------|
| Operating system / system details (`uname -s`, `sw_vers`) | Which OS and version the computer is running | The system is Darwin (the core of macOS). macOS version 26.6.2 |
| Current account identity (`whoami`) | Which user account is running my commands, and so which files and permissions I have | The account name is [redacted] |
| Available and used storage (`df -h /`) | How much disk space is total, used and free | Total: 460 GB, used: 12 GB, available: 368 GB |
| System activity snapshot (`top -l 1`) | A one-time view of CPU use, memory use and the busiest processes | CPU was about 21% busy (78.85% idle) and about 15 GB of memory was in use. There were 806 processes, 3 of them running. |

### Task 3.2 — Processes
I opened Chrome and ran `ps -e` to see the process list. The first column is the PID, and the last column (CMD) shows the program that is running. I could see processes such as launchd and Google Chrome.

- **What is a process?** A process is a program that is currently running. When I open an app, the OS starts a process for it and gives it memory and CPU time.
- **What does the PID column represent?** The PID (process identifier) is a unique number the OS gives each running process, so it can track and manage it.
- **Two example processes on my computer:** launchd (PID 1), which macOS starts first and which starts other processes, and Google Chrome, my web browser, which runs as several processes.

### Task 3.3 — Paths and permissions
I moved from the project folder into `mission-02-terminal` and then into `terminal-practice`, running `pwd` each time. The path got longer each time I went deeper into the folders.

- **Absolute path:** the full address of a file starting from the root of the computer. Example from my assignment: `/Users/[redacted]/Documents/digital-detective-8480/mission-02-terminal/README.md`.
- **Relative path:** the address of a file starting from the folder I am currently in. Example: from the project folder, `mission-02-terminal/README.md`.

I ran `ls -l notes.txt` inside `terminal-practice`. The permission letters were `-rw-r--r--`. For the owner, the letters are `rw-`, so the owner can read and write the file but cannot execute it. The group and others have `r--`, so they can only read it. I did not change any permissions.

### Task 3.4 — Operating-system responsibilities

| OS responsibility | Your explanation | Example |
|-------------------|------------------|---------|
| Process management | Decides which programs run, starts and stops them, and shares CPU time between them | Running Chrome and VS Code at the same time |
| Memory management | Gives each program the RAM it needs and takes it back when the program closes | Closing a big app frees memory for others |
| Device management | Controls hardware like the keyboard, screen and speakers through drivers | Pressing a key shows a letter on the screen |
| File management | Organises files and folders and keeps track of where they are stored | Saving README.md in a folder on the SSD |
| User interface / shell | Lets me interact with the computer, using a graphical desktop or a command-line shell | Using Finder with the mouse, or typing commands in the zsh Terminal |
| Security and permissions | Controls who can read, change or run files and protects the system | Normal users cannot change system files without permission |

## 3. Commands / tools used
- `uname -s`: shows the OS kernel name.
- `sw_vers`: shows the macOS version.
- `whoami`: shows the current user account (output not published).
- `df -h /`: shows disk space in readable units.
- `top -l 1 | head -12`: shows a one-time snapshot of system activity.
- `ps -e`: lists running processes with their PIDs.
- `grep -i chrome`: filters the process list to lines containing "chrome".
- `head`: shows only the first lines of output.
- `pwd`, `cd`: show and change the current folder.
- `ls -l`: shows a detailed listing including permissions.
- Git: `git add`, `git commit`, `git push` to save the mission.

## 4. My understanding
The operating system sits between the hardware and the programs I use. It starts programs as processes, gives them memory, controls devices, manages files and enforces permissions. A process is a running program, and each has a PID so the OS can keep track of it. A path is the address of a file. An absolute path starts from the root, while a relative path starts from where I am now. Permissions r, w and x decide whether a file can be read, changed or run, and they protect files from being changed by mistake.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-03-operating-system/README.md`

No screenshots or raw command output were added, because the output shows my username and device details.

## 8. Commit details
Commit message: "Document operating system and file management"

The work was pushed to GitHub and I confirmed the file and commit are visible.