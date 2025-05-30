## 🧪 Lab: Loops & Functions in Bash

### 🎯 Objective:

Learn how to create and use **loops** (`for`, `while`) and **functions** in Bash using `vi`.

---

## 📘 Part 1: Loops

### 🔁 Example 1: `for` Loop

---

### 🛠️ Create the Script:

```bash
vi for_loop.sh
```

### ✍️ Code:

```bash
#!/bin/bash

echo "Numbers from 1 to 5 using for loop:"
for i in {1..5}
do
    echo "Number: $i"
done
```

### ▶️ Run the Script:

```bash
chmod +x for_loop.sh
./for_loop.sh
```

### 📌 Explanation:

* `{1..5}` generates numbers 1 to 5
* Each number is printed in the loop

---

### 🔁 Example 2: `while` Loop

```bash
vi while_loop.sh
```

### ✍️ Code:

```bash
#!/bin/bash

count=1
while [ $count -le 5 ]
do
    echo "Count is: $count"
    ((count++))
done
```

### ▶️ Run:

```bash
chmod +x while_loop.sh
./while_loop.sh
```

### 📌 Explanation:

* Initializes `count` to 1
* Loops until count is greater than 5
* `((count++))` increments the counter

---

## 📘 Part 2: Functions

---

### 🛠️ Create Script with a Function:

```bash
vi function_example.sh
```

### ✍️ Code:

```bash
#!/bin/bash

# Function to greet user
greet_user() {
    echo "Hello, $1! Welcome to the Bash scripting lab."
}

# Calling function with argument
echo "Enter your name:"
read name

greet_user "$name"
```

### ▶️ Run:

```bash
chmod +x function_example.sh
./function_example.sh
```

### 📌 Explanation:

* `greet_user()` is a function that accepts an argument (`$1`)
* The function is called with the user’s input name

---

## 🧠 Summary

| Concept       | Key Point                                  |
| ------------- | ------------------------------------------ |
| `for` loop    | Repeats a block a specific number of times |
| `while` loop  | Repeats while a condition is true          |
| Function      | Reusable block of code                     |
| `$1`, `$2`,.. | Positional arguments to functions          |

