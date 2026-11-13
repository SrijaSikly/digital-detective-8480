# Mission 5 — Numbers and data

## 1. Task / objective
The task was to convert numbers between decimal, binary and hexadecimal by hand, verify the answers with Python, build a small number converter program, and explain how text is stored using encoding.

## 2. Work completed

### Task 5.1 — Manual conversions

| Question | Your working and answer |
|----------|-------------------------|
| Decimal 13 to binary | Divide by 2 and note remainders: 13÷2 = 6 r **1**, 6÷2 = 3 r **0**, 3÷2 = 1 r **1**, 1÷2 = 0 r **1**. Read the remainders from bottom to top: **1101** |
| Decimal 25 to binary | 25÷2 = 12 r **1**, 12÷2 = 6 r **0**, 6÷2 = 3 r **0**, 3÷2 = 1 r **1**, 1÷2 = 0 r **1**. Bottom to top: **11001** |
| Binary 1010 to decimal | Place values 8, 4, 2, 1: (1×8) + (0×4) + (1×2) + (0×1) = 8 + 2 = **10** |
| Binary 1101 to decimal | (1×8) + (1×4) + (0×2) + (1×1) = 8 + 4 + 1 = **13** |
| Hexadecimal A to decimal | A stands for 10, so the answer is **10** |
| Hexadecimal 1F to decimal | (1×16) + (F×1) = 16 + 15 = **31** |
| Binary 1111 to hexadecimal | 1111 is 8 + 4 + 2 + 1 = 15, and 15 is F in hexadecimal, so the answer is **F** |

### Task 5.2 — Verification using Python

| Expression tested | Result | Matches my manual answer? |
|-------------------|--------|---------------------------|
| `bin(13)` | `'0b1101'` | Yes (1101) |
| `bin(25)` | `'0b11001'` | Yes (11001) |
| `int('1010', 2)` | `10` | Yes |
| `int('1101', 2)` | `13` | Yes |
| `hex(31)` | `'0x1f'` | Yes (1F is 31) |
| `int('A', 16)` | `10` | Yes |
| `int('1F', 16)` | `31` | Yes |
| `hex(15)` | `'0xf'` | Yes (1111 is F) |

### Task 5.3 — Number converter
I created `number_converter.py`. It asks for a decimal number, converts it with `int()`, `bin()` and `hex()`, and prints both results.

| Test number | Binary output | Hexadecimal output |
|-------------|---------------|--------------------|
| 10 | 0b1010 | 0xa |
| 25 | 0b11001 | 0x19 |
| 255 | 0b11111111 | 0xff |

- `input()` reads what the user types, as text.
- `int()` turns that text into a whole number.
- `bin()` converts a number to a binary string starting with `0b`.
- `hex()` converts a number to a hexadecimal string starting with `0x`.

### Task 5.4 — How is text stored?
- ASCII code for uppercase **A** is **65**, and for lowercase **a** it is **97** (I checked with `ord()` in Python).
- A computer only stores numbers (bits), so it needs an encoding standard that says which number stands for which character. Without it, different computers could read the same bits as different letters.
- An example of a character not in basic ASCII is the rupee sign **₹**. UTF-8 can represent it, and many other symbols and languages.

## 3. Commands / tools used
- `python3`: opened Python's interactive environment.
- `bin()`, `hex()`: convert a number to binary or hexadecimal text.
- `int(text, base)`: converts binary or hexadecimal text to a decimal number.
- `ord()`: gives the ASCII/Unicode number of a character.
- `input()`, `print()`: used in the converter to read and show values.
- `python3 mission-05-numbers-data/number_converter.py`: ran the converter.
- VS Code: used to write the program and README.
- Git: `git add`, `git commit`, `git push` to save the mission.

## 4. My understanding
Computers store everything as bits, which are 0s and 1s. Binary is base 2, decimal is base 10 and hexadecimal is base 16. To convert decimal to binary I divide by 2 and read the remainders backwards, and to convert binary to decimal I add up the place values (8, 4, 2, 1). Hexadecimal is a shorter way to write binary, because one hex digit stands for four bits. Python's built-in functions let me check my hand calculations. Text is also stored as numbers, using encodings such as ASCII and UTF-8.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-05-numbers-data/README.md`
- `mission-05-numbers-data/number_converter.py`

## 8. Commit details
Commit message: "Build number converter and practise data representation"

The work was pushed to GitHub and I confirmed the files and commit are visible.