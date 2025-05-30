## 🔬 **Lab: Using Command Substitution in Bash**

## 📘 **What is Command Substitution?**

Command substitution allows the output of a command to be **stored in a variable** or **embedded within another command**.

### 🔧 Syntax:

```bash
variable=$(command)
# or
variable=`command`  # Backticks (deprecated, but still works)
```

---

## 🛠️ **Lab Steps Using `vi` Editor**

---

### 1️⃣ Step 1: Open Terminal and Create Script Using `vi`

```bash
vi cmdsub_example.sh
```

---

### 2️⃣ Step 2: Press `i` to enter **INSERT MODE**, and type the following script:

```bash
#!/bin/bash

# Command substitution to get current date
current_date=$(date)

# Get current username
user_name=$(whoami)

# Output the collected information
echo "Hello, $user_name!"
echo "Today's date is: $current_date"
```

---

### 3️⃣ Step 3: Save and Exit `vi`

* Press `Esc`
* Type `:wq` and press `Enter` to **write and quit**

---

### 4️⃣ Step 4: Make the Script Executable

```bash
chmod +x cmdsub_example.sh
```

---

### 5️⃣ Step 5: Run the Script

```bash
./cmdsub_example.sh
```

---

### 🟢 **Expected Output (example)**

```
Hello, ninad!
Today's date is: Fri May 30 13:25:43 IST 2025
```

