# Minishell

A lightweight shell implementation written in **C** as part of the **42 Network curriculum**.  
The goal is to rebuild a simplified version of **bash** to learn parsing, processes, file descriptors, and env management.

## ✨ Features
- Prompt display & command parsing
- Built-ins: `cd`, `echo`, `pwd`, `export`, `unset`, `env`, `exit`
- External programs via `execve`
- Pipes (`|`) for command chaining
- I/O redirection (`<`, `>`, `>>`)
- Environment variable expansion (`$VAR`, `$?`)
- Signal handling (e.g., `Ctrl-C`, `Ctrl-\`, **`Ctrl-D` for EOF**)
- Exit status behavior similar to bash

## 🛠️ Tech Stack
- **Language:** C
- **Build:** Makefile
- **Libraries:** [Libft](./Libft)

> Requires **readline**.
> - macOS: `brew install readline` then `CPPFLAGS="-I$(brew --prefix readline)/include" LDFLAGS="-L$(brew --prefix readline)/lib" make`
> - Debian/Ubuntu: `sudo apt-get install libreadline-dev && make`


## 🚀 Usage

### 1) Clone
```bash
git clone https://github.com/Dimi20cen/42-minishell.git
cd 42-minishell
````

### 2) Build

```bash
make
```

### 3) Run

```bash
./minishell
```

## 📂 Project Structure

* `src/` → source code
* `header/` → header files
* `Libft/` → custom utility library
* `Makefile` → build rules
* `Subject.pdf` → original 42 requirements


## 📖 Learning Outcomes

* `fork`, `exec*`, `wait*` process control
* File descriptors, pipes, redirections
* Tokenization & quoting rules
* UNIX signal handling
* Building an interactive C program
