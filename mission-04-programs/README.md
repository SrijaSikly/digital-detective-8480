# Mission 4 — How programs run

## 1. Task / objective
The task was to create and run a simple Python program, and to compare how a compiler and an interpreter translate or execute programs.

## 2. Work completed

### Task 4.1 — Create and run a Python program
I created `hello.py` inside `mission-04-programs`. It has one line: `print("Hello from Python")`. I ran it from Terminal with `python3 mission-04-programs/hello.py` and the message "Hello from Python" appeared, so the program works.

### Task 4.2 — Compare compiler and interpreter

| Point | Compiler | Interpreter |
|-------|----------|-------------|
| When translation / execution happens | The whole program is translated before it runs | The program is read and executed line by line while it runs |
| Typical output | A separate executable (machine code) file | No separate file, the result of running the program appears directly |
| One example | GCC (compiles C programs) | The Python interpreter (`python3`) |
| One advantage | The compiled program usually runs faster | It is easy to run and test code quickly, with no separate build step |

Explanation:
A compiler translates the whole source code into another form, usually machine code, before the program runs, so I get a ready-to-run file. An interpreter reads the program and carries out its instructions while it is running, line by line. This is why I could run `hello.py` straight away with `python3` without any build step. In real life, many languages use a mix of both ideas, so the difference is not always strict.

## 3. Commands / tools used
- `cd`: moved to the project folder.
- `echo` with `>`: created `hello.py` with one line of code.
- `cat`: displayed the file to check its contents.
- `python3`: ran the program with the Python interpreter.
- VS Code: used to write the README.
- Git: `git add`, `git commit`, `git push` to save the mission.

## 4. My understanding
A program written in Python or C language is just text until the computer can run it. A compiler converts all of it to machine code first, while an interpreter runs it directly as it goes. Compiled programs tend to run faster, while interpreted programs are quicker to write and test. Python is usually run through an interpreter, which is why one command was enough to run my program.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-04-programs/hello.py`
- `mission-04-programs/README.md`

## 8. Commit details
Commit message: "Compare compilers and interpreters"

The work was pushed to GitHub and I confirmed the files and commit are visible.