# Mission 6 — Git and GitHub

## 1. Task / objective
The task was to understand version control, stage and commit changes, create a branch, open a Pull Request on GitHub, and explain the collaboration workflow.

## 2. Work completed

### Task 6.1 — Basic Git workflow

| Git operation | What it does in my own words |
|---------------|------------------------------|
| Check repository status (`git status`) | Shows which branch I am on and which files are changed, staged or untracked |
| Stage selected changes (`git add <file>`) | Chooses which changed files will go into the next commit |
| Create a commit (`git commit -m "..."`) | Saves a snapshot of the staged files in the history with a message |
| View commit history (`git log --oneline`) | Lists the earlier commits, one line each, newest first |

**Staging vs committing:** staging picks which changes to include, and committing records those staged changes permanently in the history. I can stage several files, check them, and then commit them together.

### Task 6.2 — Branch
I created a branch called `update-about` with `git switch -c update-about`. On it I added a "My Learning" section to the root README, staged it, committed it with the message "Add My Learning section to README", and published the branch with `git push -u origin update-about`.

### Task 6.3 — Pull Request
I opened a Pull Request from `update-about` into `main` on GitHub with the title "Add My Learning section to README" and reviewed the changed file.

**PR status:** [WRITE ONE: "Merged into main" OR "Open, not merged, because my instructor did not ask me to merge it"].

- **Branch:** a separate line of work that lets me change files without touching the main version.
- **Pull Request:** a request on GitHub to bring the changes from one branch into another, so others can review them first.
- **Why useful:** when several people work on one project, each can work on their own branch, and the team can review changes in a PR before merging, which avoids breaking the main code.

### Task 6.4 — Git command glossary

| Operation | One-line explanation |
|-----------|----------------------|
| Initialise a repository (`git init`) | Turns a folder into a Git repository so changes can be tracked |
| Check status (`git status`) | Shows changed, staged and untracked files |
| Stage changes (`git add`) | Marks files to be included in the next commit |
| Commit changes (`git commit`) | Saves the staged changes as a snapshot with a message |
| View history (`git log`) | Shows the list of past commits |
| Create or list branches (`git branch`, `git switch -c`) | Lists branches, or creates a new one and switches to it |
| Switch branches (`git switch`) | Moves me to another branch |
| Publish changes (`git push`) | Uploads my local commits to GitHub |
| Retrieve remote changes (`git pull`) | Downloads new changes from GitHub and merges them into my branch |

## 3. Commands / tools used
- `git status`, `git add`, `git commit`, `git log --oneline`, `git branch`, `git switch -c`, `git switch`, `git push -u origin update-about`, `git restore --staged`, `git pull` (only if merged).
- GitHub website: to create and review the Pull Request.
- VS Code: to edit the README files.

## 4. My understanding
Git records the history of my project. I stage the changes I want, then commit them as a snapshot. A branch lets me try a change safely, and a Pull Request lets the change be reviewed before it joins `main`. GitHub hosts the repository online so work can be shared and reviewed.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-06-git-github/README.md`
- Branch `update-about` and its Pull Request, visible on GitHub.

## 8. Commit details
Commit message: "Complete Git and GitHub collaboration mission"

The work was pushed to GitHub and I confirmed the files and commit are visible.
