## 🧪 Lab: Comparison and Logical Operators in Bash

### 🧠 Objective:

Understand how to use **comparison** and **logical** operators to control flow in Bash scripts.

---

## 📘 Part 1: Comparison Operators

### 🔧 Common Numeric Comparison Operators:

| Operator | Meaning                  |
| -------- | ------------------------ |
| `-eq`    | Equal to                 |
| `-ne`    | Not equal to             |
| `-gt`    | Greater than             |
| `-lt`    | Less than                |
| `-ge`    | Greater than or equal to |
| `-le`    | Less than or equal to    |

---

### 🛠️ Create Script for Comparison

```bash
vi compare.sh
```

### ✍️ Code:

```bash
#!/bin/bash

echo "Enter your age:"
read age

if [ $age -ge 18 ]; then
    echo "You are eligible to vote."
else
    echo "You are NOT eligible to vote."
fi
```

### ✅ Steps to Run:

```bash
chmod +x compare.sh
./compare.sh
```

### 📌 Explanation:

* Takes age input
* Uses `-ge` (greater than or equal to) to check voting eligibility

---

## 📘 Part 2: Logical Operators

### 🔧 Bash Logical Operators:

| Operator | Meaning                           |    |            |
| -------- | --------------------------------- | -- | ---------- |
| `&&`     | Logical AND                       |    |            |
| \`       |                                   | \` | Logical OR |
| `!`      | Logical NOT (used inside `[[ ]]`) |    |            |

---

### 🛠️ Create Script for Logical Operators

```bash
vi logical.sh
```

### ✍️ Code:

```bash
#!/bin/bash

echo "Enter username:"
read username

echo "Enter age:"
read age

if [[ "$username" == "admin" && $age -ge 18 ]]; then
    echo "Access granted."
else
    echo "Access denied."
fi
```

### ✅ Steps to Run:

```bash
chmod +x logical.sh
./logical.sh
```

