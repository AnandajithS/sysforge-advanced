
# SysForge Advanced– Rebuilding the Unix Core

Welcome to **SysForge**, a challenge where you step into the shoes of a system explorer, diving deep into the broken-down world of Unix. The core command-line tools that once powered this world (`ls`, `wc`, `cat`, and `grep`) are gone.

Your mission: **Rebuild them from scratch using C**, and bring order back to the terminal!

Instead of just using these tools, you’ll create simplified versions of them, give them custom names, and make them work just like the originals with **extra flags**, **multiple file support**, and **error handling** 

---

## Objective

Recreate the following core Unix commands with your own C programs:

| Custom Command | Original Equivalent | Description                          |
|----------------|---------------------|--------------------------------------|
| `listit`       | `ls`                | List files in a directory            |
| `showtext`     | `cat`               | Display contents of files            |
| `countit`      | `wc`                | Count lines, words, and characters   |
| `finder`       | `grep`              | Search for text inside files         |

Each command should be a **separate executable** and should work **from the terminal**, just like real Unix commands.

---

## Flags to Implement

### `listit`
- `-a` : Show all files, including hidden ones  
- `-l` : Show detailed file info (permissions, size, etc.)  
- `-1` : List one file per line  
- `-r` : Reverse file order  
- `--help` : Show a custom help message  

### `showtext`
- `-n` : Number all lines  
- `-b` : Number non-empty lines only  
- `-s` : Squeeze multiple blank lines into one  
- `-e` : Show `$` at the end of lines  
- `--help` : Show a custom help message  

### `countit`
- `-l` : Count lines  
- `-w` : Count words  
- `-c` : Count characters  
- `-L` : Show length of longest line  
- `--help` : Show a custom help message

### `finder`
- `-i` : Ignore case while matching  
- `-n` : Show line numbers for matches  
- `-v` : Show only non-matching lines  
- `-c` : Show count of matching lines  
- `--help` : Show a custom help message


## Requirements

- Each command must be implemented as a **separate C file** 
- Must work with **multiple files or directories** (where applicable).
- Your command must handle:
  - Invalid or missing arguments
  - Invalid flags
  - File not found or permission errors
- Implement `--help` for each command to print the usage instructions

    eg. **listit --help**

    ```bash
    Usage: listit [OPTIONS] [directory1] [directory2] ...

    List files in the specified directory (or current directory by default).

    Options:
    -a            Show all files, including hidden ones
    -l            Show detailed file info (permissions, size, etc.)
    -1            List one file per line
    -r            Reverse the order of files
    --help    Show this help message and exit
    ```


