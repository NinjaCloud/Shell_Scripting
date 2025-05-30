## 🧪 1️⃣ **Example: `if` Statement**


### 🛠️ Steps:

```bash
vi if_example.sh
```

### ✍️ Code:

```bash
#!/bin/bash

echo "Enter a number:"
read num

if [ $num -gt 100 ]; then
    echo "The number is greater than 100."
fi
```

### ✅ Run:

```bash
chmod +x if_example.sh
./if_example.sh
```

---

## 🧪 2️⃣ **Example: `if-else` Statement**

### 🔧 Objective: Check if a user is root or not

---

### 🛠️ Steps:

```bash
vi if_else_example.sh
```

### ✍️ Code:

```bash
#!/bin/bash

user=$(whoami)

if [ "$user" == "root" ]; then
    echo "You are the root user."
else
    echo "You are a regular user."
fi
```

### ✅ Run:

```bash
chmod +x if_else_example.sh
./if_else_example.sh
```

---

## 🧪 3️⃣ **Example: `if-elif-else` Statement**

### 🔧 Objective: Categorize a number as positive, negative, or zero

---

### 🛠️ Steps:

```bash
vi if_elif_else_example.sh
```

### ✍️ Code:

```bash
#!/bin/bash

echo "Enter a number:"
read num

if [ $num -gt 0 ]; then
    echo "Positive number"
elif [ $num -lt 0 ]; then
    echo "Negative number"
else
    echo "Zero"
fi
```

### ✅ Run:

```bash
chmod +x if_elif_else_example.sh
./if_elif_else_example.sh
```

