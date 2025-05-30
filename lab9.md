## 🧪 Lab: File Operations & Error Handling in Bash

### 🎯 Objective:

* Learn to check if a file exists.
* Read from and write to a file.
* Handle errors (e.g., file not found).

---

## 📘 Script Name: `file_operations.sh`

---

### 🛠️ Step 1: Open `vi` to Create the Script

```bash
vi file_operations.sh
```

---

### ✍️ Script Code:

```bash
#!/bin/bash

# File name
filename="sample.txt"

# Check if file exists
if [ -f "$filename" ]; then
    echo "File $filename exists."
else
    echo "File $filename not found. Creating it now..."
    touch "$filename"
    if [ $? -ne 0 ]; then
        echo "Error: Unable to create the file."
        exit 1
    fi
fi

# Write to the file
echo "This is a test message written to $filename." >> "$filename"

# Read the file
echo "Contents of $filename:"
cat "$filename"
```

---

### ✅ Step 2: Save & Exit

Press `Esc`, then type:

```
:wq
```

---

### ▶️ Step 3: Make the Script Executable

```bash
chmod +x file_operations.sh
```

---

### ▶️ Step 4: Run the Script

```bash
./file_operations.sh
```

---

## 📌 Explanation

| Line                    | Purpose                                |
| ----------------------- | -------------------------------------- |
| `if [ -f "$filename" ]` | Checks if file exists                  |
| `touch "$filename"`     | Creates file if not found              |
| `$?`                    | Checks the exit status of last command |
| `>> "$filename"`        | Appends a message to the file          |
| `cat "$filename"`       | Displays file content                  |

---

