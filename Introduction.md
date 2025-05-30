# **Introduction to Bash**

**Bash** (Bourne Again SHell) is a Unix shell and command language written as a free software replacement for the Bourne shell (sh). It is the default shell in most Linux distributions and macOS. Bash allows users to interact with the system by typing commands, running scripts, and automating administrative tasks. It supports features like command history, command completion, and job control, making it powerful for both interactive use and scripting.

---

### **History of Bash**

Bash was developed by **Brian Fox** in **1989** for the **GNU Project** as a free alternative to the Bourne Shell. It incorporated features from other popular shells like **ksh (KornShell)** and **csh (C Shell)**. Over time, Bash became the most widely used shell across Linux distributions due to its compatibility, extensibility, and strong community support. It is maintained by the Free Software Foundation.

---

### **Bash Files – `.bash_profile`**

* `.bash_profile` is executed for **login shells**.
* It is used to set **environment variables**, **PATH**, and execute commands that should run once at login.
* Typical use cases include setting up custom environments, aliases, and startup programs.
* It is located in the user's home directory (`~/.bash_profile`).

---

### **Bash Files – `.bashrc`**

* `.bashrc` is executed for **non-login interactive shells**, like when you open a new terminal window.
* It’s commonly used to define **aliases**, **functions**, **prompt settings**, and other interactive shell configurations.
* Even though it's not run for login shells by default, `.bash_profile` often includes a line to source `.bashrc` for consistency.
* Path: `~/.bashrc`

---

### **Bash Files – `.bash_history`**

* `.bash_history` stores the **history of commands** executed by the user in Bash.
* Located at `~/.bash_history`, it allows users to access and reuse previous commands using the `history` command or shortcuts like the up arrow key.
* History settings (like the number of stored commands) can be controlled via environment variables such as `HISTSIZE` and `HISTFILESIZE`.

---

### **Bash Files – `.bash_logout`**

* `.bash_logout` is executed when a **login shell exits**.
* Common uses include clearing the screen, logging out messages, or performing clean-up operations.
* Example: `clear` command to clean the terminal when a user logs out.
* Path: `~/.bash_logout`


