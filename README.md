
# SysForge Advanced– Rebuilding the Unix Core

Welcome to **SysForge**, a challenge where you step into the shoes of a system explorer, diving deep into the broken-down world of Unix. The core command-line tools that once powered this world (`ls`, `wc`, `cat`, and `grep`) are gone.

Your mission: **Rebuild them from scratch using C**, and bring order back to the terminal!

Instead of just using these tools, you’ll create simplified versions of them, give them custom names, and make them work just like the originals with **multiple flags**, **multiple file support**, and **error handling** 

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
- `-1` : List one file per line  
- `-r` : Reverse file order  

### `showtext`
- `-n` : Number all lines  
- `-s` : Squeeze multiple blank lines into one  
- `-e` : Show `$` at the end of lines  

### `countit`
- `-l` : Count lines  
- `-w` : Count words  
- `-c` : Count characters  

### `finder`
- `-n` : Show line numbers for matches  
- `-v` : Show only non-matching lines  
- `-c` : Show count of matching lines  


## Requirements

- Each command must be implemented as a **separate C file** 
- Must work with **multiple files or directories** (where applicable).
- Must support multiple flags used separately (e.g., `listit -a -r`)
  - Combined (e.g., `listit -ar`) flags are optional
- Your commands must be **runnable from anywhere in the terminal**, like the original Unix tools.
- Your command must handle:
  - Invalid or missing arguments
  - Invalid flags
  - File not found or permission errors

---

## Writeups

Along with your code, include a **brief writeup for each command** that covers:
- Your approach to building it  
- Any challenges or bugs you encountered  
- What you learned during the process

---

Happy forging, and may your terminal tools shine bright again! 

