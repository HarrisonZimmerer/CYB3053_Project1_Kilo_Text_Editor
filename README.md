# CYB Project 1 Kilo Text Editor — From Scratch 
## Objective

The goal of this project was to build a fully functional text editor from scratch in C, following the tutorial [*“Build Your Own Text Editor”*](https://viewsourcecode.org/snaptoken/kilo/).

Through this process, I gained hands-on experience with system calls, terminal control, and low-level I/O — core concepts for understanding how operating systems interact with user programs.

The end result is a minimalist text editor based on *antirez’s kilo* (~1000 lines of C in a single file) with features like syntax highlighting and incremental search.

### Skills Learned

* Writing and compiling C programs on Linux
* Understanding and using system calls (read, write, open, close, tcgetattr, tcsetattr, etc.)
* Working with terminal raw mode and low-level input/output
* Implementing file I/O for text editing
* Understanding how text editors manage buffers and cursor movement
* Syntax highlighting implementation
* Basic search functionality in a terminal application
* Using `gcc` and `Makefile` to build projects

### Tools Used

* C (GCC) – Language and compiler
* Terminal / TTY – For raw input/output control
* Vim / VS Code – Editor for writing C code
* Git & GitHub – Version control and project tracking
* Unix System Calls – For low-level interaction with the OS

---

## Features 

* Terminal raw mode (no line buffering)
* Cursor movement with arrow keys
* Text editing (insert/delete)
* File loading and saving
* Incremental search within the file
* Basic syntax highlighting
* Single-file C implementation (~1000 LOC)
* Runs entirely in the terminal

---

## Installation & Setup 🧭

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/kilo-text-editor.git
cd kilo-text-editor
```

### 2. Build the Editor

```bash
gcc kilo.c -o kilo -Wall -Wextra -pedantic -std=c99
```

(Or use the included `Makefile` if provided)

```bash
make
```

### 3. Run the Editor

```bash
./kilo [filename]
```

If the file does not exist, it will be created when you save.

---

## Usage 📝

### Basic Commands

| Key                | Action            |
| ------------------ | ----------------- |
| Arrow Keys         | Move cursor       |
| Ctrl-S             | Save file         |
| Ctrl-Q             | Quit editor       |
| Ctrl-F             | Search text       |
| Text Input         | Insert characters |
| Backspace / Delete | Remove characters |

### Example

```bash
./kilo notes.txt
```

This opens or creates `notes.txt` in the editor.

---


## Credits
* Project provided by: University of Tulsa — CYB-3053: Operating Systems Concepts
* Tutorial: [Build Your Own Text Editor](https://viewsourcecode.org/snaptoken/kilo/) by snaptoken
* Original code inspiration: [antirez’s kilo](https://github.com/antirez/kilo)

---

## License

This project was completed for educational purposes.
The code is adapted from an open tutorial and is free to modify, extend, or distribute under an open-source license.

---

✅ *[Read the tutorial here →](https://viewsourcecode.org/snaptoken/kilo/)*

