## 🔬 **Lab: Print Output in Bash Scripting**

### 🧠 **Objective**

Understand how to **print messages or data** to the terminal using `echo` and `printf` in a Bash script.

---

## 🧾 **Using `echo`**

### 🔍 What is `echo`?

* `echo` is a built-in Bash command used to **display a line of text** or a variable value.
* Syntax:

  ```bash
  echo [option] [string]
  ```

---

### ✍️ **Create a Script Using `echo`**

#### 1️⃣ Step 1: Open terminal and create a file

```bash
nano echo_example.sh
```

#### 2️⃣ Step 2: Add the following code

```bash
#!/bin/bash

# Print a static message
echo "Welcome to Bash Scripting!"

# Print a variable
name="Ninad"
echo "Hello, $name!"

# Print with special characters
echo "Today's date: $(date)"
```

#### 3️⃣ Step 3: Save, make executable, and run

```bash
chmod +x echo_example.sh
./echo_example.sh
```

🟢 **Expected Output:**

```
Welcome to Bash Scripting!
Hello, Ninad!
Today's date: Fri May 30 13:10:00 IST 2025
```




