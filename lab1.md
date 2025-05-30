## 🔬 **Lab: Understanding Shebang Line & Comments in Bash Scripts**

## 🧾 **Part 1: Shebang Line (`#!`)**

### 🔍 What is it?

* The **Shebang line** tells the system **which interpreter** to use to run the script.
* It is **always the first line** in the script.
* Syntax:

  ```bash
  #!/path/to/interpreter
  ```

### ✅ Most common shebang for Bash:

```bash
#!/bin/bash
```

---

## ✍️ **Create a Bash Script Using Shebang**

### 1️⃣ Step 1: Open terminal and create a new script

```bash
nano shebang_example.sh
```

### 2️⃣ Step 2: Write the following code:

```bash
#!/bin/bash

# This script shows the current date and time
echo "Today's date is: $(date)"
```

### 3️⃣ Step 3: Save and exit (`Ctrl + O`, `Enter`, then `Ctrl + X`)

### 4️⃣ Step 4: Make the script executable

```bash
chmod +x shebang_example.sh
```

### 5️⃣ Step 5: Run the script

```bash
./shebang_example.sh
```

🟢 **Expected Output:**

```
Today's date is: Fri May 30 12:45:00 IST 2025
```

---

## 🧾 **Part 2: Comments in Bash**

### 🔍 What are comments?

* Lines that start with `#` (except the shebang line) are **ignored by the shell**.
* Used for **documentation**, **explanation**, or **disabling code temporarily**.

### ✅ Example:

```bash
#!/bin/bash

# This is a comment
# Print the username
echo "Current user is: $USER"
```


