## Bandit Level Notes

### Level 0
* **`ssh username@hostname -p port`** – Connects to network services remotely.

### Level 0 → Level 1
* **`cat file`** – Prints the content of a file.
* **`exit`** – Closes the current SSH session so you can log into the next level.

### Level 1 → Level 2
* **Handling `-` filenames:** You cannot use `cat -` directly because `-` means stdin. Use `./-` instead.

### Level 2 → Level 3
* **Filenames with spaces:** Wrap the filename in quotes or put `--` before the filename (e.g., `cat -- "file name"`).

### Level 3 → Level 4
* **`cd directory`** – Navigates to a specific directory.
* **`ls -la`** – Lists all files in detail, including hidden files (files starting with `.`).

### Level 4 → Level 5
* **`file filename`** – Reveals the true file type of a file.
* **`*` wildcard** – Expands to include every file in the current directory.

### Level 5 → Level 6
* **`find . -type f`** – Searches the current directory (`.`) for regular files (`-type f`).

### Level 6 → Level 7
* **`find /`** – Searches starting from the root directory (`/`).

### Level 7 → Level 8
* **`grep 'pattern' file`** – Searches and prints lines matching a specific pattern.

### Level 8 → Level 9
* **`sort file | uniq -u`** – `uniq` only checks adjacent lines, so you must pipe `sort` into `uniq -u` to extract unique lines.

### Level 9 → Level 10
* **`strings file`** – Extracts human-readable text from binary data.

### Level 10 → Level 11
* **`base64 -d file`** – Decodes Base64 encoded data back to plain text.

### Level 11 → Level 12
* **`tr 'A-Za-z' 'N-ZA-Mn-za-m'`** – Decodes ROT13 shifted text.

### Level 12 → Level 13
* **`mktemp -d`** – Creates a unique temporary directory inside `/tmp`.
* **`cp source destination`** – Copies a file to a target directory.
* **`xxd -r input > output`** – Reverts a hex dump back into binary data.
* **`gzip -d file.gz`** – Decompresses `.gz` files.
* **`bzip2 -d file.bz2`** – Decompresses `.bz2` files.
* **`tar -xf file.tar`** – Extracts `.tar` archive files.
