BigShell
========
Big Shell is a custom Unix-like command-line shell implemented in C. It supports job control, process management, built-in commands, and basic shell 
features. This project was developed as part of a systems programming course to deepen understanding of process handling, signals, and terminal control.

## Features

- Execute external programs with arguments
- Built-in commands:
  - `cd` – change the current directory
  - `exit` – exit the shell
  - `jobs` – list background jobs
  - `fg` – bring a job to the foreground
  - `bg` – resume a job in the background
- Job control:
  - Supports running jobs in foreground and background
  - Handles stopped and terminated processes
  - Tracks job status
- Signal handling:
  - Properly handles `SIGINT` (Ctrl-C) and `SIGTSTP` (Ctrl-Z)
- Command history (optional depending on implementation)

## Installation

Clone the repository and build the shell using `make`:

```bash
git clone https://github.com/YourUsername/big-shell.git
cd big-shell
make


Makefile:
 
.. code-block:: console

   $ make          # Equivalent to `make all`
   $ make all      # Equivalent to `make release debug` (default target)
   $ make release  # Release build in release/ -- no debugging messages
   $ make debug    # Debug build in debug/ -- includes assertions and debugging messages
   $ make clean    # Removes build files (release/ and debug/ directories)
