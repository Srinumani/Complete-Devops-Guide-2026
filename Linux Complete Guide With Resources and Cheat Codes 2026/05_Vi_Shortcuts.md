# VI Editor Shortcuts 

### Modes in VI Editor
- **Normal Mode** (default) – Used for navigation and command execution.
- **Insert Mode** – Used for text editing (press `i` to enter, `Esc` to exit).
- **Command Mode** – Used for saving, quitting, and searching (press `:` in Normal mode).

---

### Basic Navigation
- `h` – Move **left**  
- `l` – Move **right**  
- `j` – Move **down**  
- `k` – Move **up**  
- `0` – Move to the **beginning** of the line  
- `^` – Move to the **first non-blank** character of the line  
- `$` – Move to the **end** of the line  
- `w` – Move to the **next word**  
- `b` – Move to the **previous word**  
- `gg` – Move to the **start** of the file  
- `G` – Move to the **end** of the file  
- `:n` – Move to **line number `n`**  

---

### Insert Mode Shortcuts
- `i` – Insert before cursor  
- `I` – Insert at the beginning of the line  
- `a` – Append after cursor  
- `A` – Append at the end of the line  
- `o` – Open a new line below  
- `O` – Open a new line above  
- `Esc` – Exit insert mode  

---

### Editing Text
- `x` – Delete a **character**  
- `X` – Delete a **character before cursor**  
- `dw` – Delete a **word**  
- `dd` – Delete a **line**  
- `d$` – Delete from **cursor to end of line**  
- `d0` – Delete from **cursor to beginning of line**  
- `D` – Delete from **cursor to end of line**  
- `u` – **Undo** last action  
- `Ctrl + r` – **Redo** an undone change  
- `yy` – Copy (yank) a **line**  
- `yw` – Copy (yank) a **word**  
- `p` – Paste **after** the cursor  
- `P` – Paste **before** the cursor  

---

### Search and Replace
- `/pattern` – Search **forward** for a pattern  
- `?pattern` – Search **backward** for a pattern  
- `n` – Repeat last search **forward**  
- `N` – Repeat last search **backward**  
- `:%s/old/new/g` – Replace **all occurrences** of "old" with "new"  
- `:s/old/new/g` – Replace **all occurrences** in the current line  

---

### Working with Multiple Files
- `:e filename` – Open a **new file**  
- `:w` – Save file  
- `:wq` – Save and exit  
- `:q!` – Quit **without saving**  
- `:split filename` – Split screen **horizontally** and open another file  
- `:vsplit filename` – Split screen **vertically**  
- `Ctrl + w + w` – Switch between split screens  


If vi is not installed
Check:

vi --version
Install (Ubuntu):

sudo apt install vim
Amazon Linux / RHEL:

sudo yum install vim
If you actually meant something else by “v1 editor” (tool name, app, AWS file, etc.), tell me where you saw it and I’ll guide you exactly 💡

You said:
what is apt 
ChatGPT said:
Good question 👍 — this is a must-know thing if you’re working with Linux / DevOps.

🔹 What is apt?
apt = Advanced Package Tool

It’s a package manager used in Debian-based Linux systems like:

Ubuntu

Linux Mint

Kali Linux

Debian

👉 It helps you install, update, remove, and manage software easily.

🧠 Simple meaning
Think of apt like Play Store or App Store, but for Linux — using commands instead of clicks.

📦 What does apt do?
Task	Command
Update package list	sudo apt update
Install software	sudo apt install nginx
Remove software	sudo apt remove nginx
Upgrade all packages	sudo apt upgrade
Search package	apt search docker
Show package info	apt show nginx
🛠 Example: Install vim
sudo apt update
sudo apt install vim
🔐 Why sudo with apt?
Because:

Installing/removing software affects the whole system

Only admin (root) is allowed
