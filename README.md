
# LSH - Learning Shell

This is a minimal shell implementation written in C, inspired by [Stephen Brennan’s LSH tutorial](https://brennan.io/2015/01/16/write-a-shell-in-c/). It’s a great learning project to understand how a command-line shell works under the hood.

## 🧠 What You'll Learn

By going through this project, you'll get hands-on experience with:

- 🔄 **Input loops** – Reading user input from the command line.
- 🪓 **Parsing input** – Splitting strings into commands and arguments.
- 🧩 **Built-in commands** – Handling internal commands like `cd`, `help`, and `exit`.
- 🧵 **Process creation** – Using `fork()` to create new processes.
- ⚙️ **Command execution** – Using `execvp()` to run external programs.
- ⏳ **Waiting for processes** – Using `waitpid()` to manage child process termination.

## 🔧 Features

- Executes external programs like `ls`, `echo`, `grep`, etc.
- Supports basic built-in commands:
  - `cd` – Change directory
  - `help` – Print available commands
  - `exit` – Quit the shell
- Tokenizes input using `strtok` with basic whitespace delimiters

## 📦 How to Build

Make sure you have GCC installed, then compile with:

```bash
gcc -o main main.c
