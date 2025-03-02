# **Conditional Statements in Python**

## **What are Conditional Statements?**
Conditional statements in Python allow us to **execute different blocks of code** based on certain conditions. These statements help control the flow of a program.

Python provides the following conditional statements:
1. **if statement**
2. **if-else statement**
3. **if-elif-else statement**
4. **Nested if statement**
5. **Ternary operator (short-hand if-else)**

---

## **1. if Statement**
The `if` statement checks a condition, and if the condition is **True**, it executes a block of code.

### **Syntax:**
```python
if condition:
    # Code to execute if condition is True
```

### **Example:**
```python
age = 18

if age >= 18:
    print("You are an adult.")  # This will execute
```

### **Explanation:**
- If `age` is `18` or more, the message `"You are an adult."` is printed.

---

## **2. if-else Statement**
The `if-else` statement adds an **alternative block** that runs when the condition is **False**.

### **Syntax:**
```python
if condition:
    # Code if condition is True
else:
    # Code if condition is False
```

### **Example:**
```python
age = 16

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")  # This will execute
```

### **Explanation:**
- If `age` is **less than 18**, it prints `"You are a minor."`

---

## **3. if-elif-else Statement**
The `if-elif-else` statement is used when there are **multiple conditions** to check.

### **Syntax:**
```python
if condition1:
    # Code if condition1 is True
elif condition2:
    # Code if condition2 is True
else:
    # Code if none of the above conditions are True
```

### **Example:**
```python
marks = 75

if marks >= 90:
    print("Grade: A")
elif marks >= 80:
    print("Grade: B")
elif marks >= 70:
    print("Grade: C")  # This will execute
else:
    print("Grade: F")
```

### **Explanation:**
- If `marks` is **75**, it falls in the `elif marks >= 70:` condition, so `"Grade: C"` is printed.

---

## **4. Nested if Statement**
You can place an `if` statement inside another `if` statement. This is called **nesting**.

### **Syntax:**
```python
if condition1:
    if condition2:
        # Code if both conditions are True
```

### **Example:**
```python
age = 20
has_id = True

if age >= 18:
    if has_id:
        print("You can enter the club.")  # This will execute
    else:
        print("You need an ID.")
else:
    print("You are too young to enter.")
```

### **Explanation:**
- The **first `if` condition (`age >= 18`)** is checked.
- If `True`, the **second `if` condition (`has_id`)** is checked.
- If both are `True`, `"You can enter the club."` is printed.

---

## **5. Ternary Operator (Short-Hand if-else)**
The **ternary operator** is a **one-line if-else statement**.

### **Syntax:**
```python
value_if_true if condition else value_if_false
```

### **Example:**
```python
age = 20
status = "Adult" if age >= 18 else "Minor"

print(status)  # Output: "Adult"
```

### **Explanation:**
- If `age >= 18`, `"Adult"` is assigned to `status`, otherwise `"Minor"`.

---

## **Comparison Operators in Conditional Statements**
Conditional statements often use **comparison operators**.

| Operator | Meaning | Example (`x = 5`, `y = 3`) |
|----------|---------|--------------------------|
| `==` | Equal to | `x == y` → `False` |
| `!=` | Not equal to | `x != y` → `True` |
| `>` | Greater than | `x > y` → `True` |
| `<` | Less than | `x < y` → `False` |
| `>=` | Greater than or equal to | `x >= y` → `True` |
| `<=` | Less than or equal to | `x <= y` → `False` |

---

## **Logical Operators in Conditional Statements**
We can also use **logical operators** in `if` conditions.

| Operator | Meaning | Example |
|----------|---------|---------|
| `and` | Both conditions must be True | `(x > 2 and x < 10)` |
| `or` | At least one condition must be True | `(x < 2 or x > 10)` |
| `not` | Reverses the condition | `not (x > 2)` |

### **Example using Logical Operators**
```python
x = 7

if x > 5 and x < 10:
    print("x is between 5 and 10.")  # This will execute
```

---

## **Summary Table**
| Statement Type | Description | Example |
|---------------|-------------|---------|
| `if` | Executes if condition is True | `if age >= 18: print("Adult")` |
| `if-else` | Runs alternative code if condition is False | `if age >= 18: print("Adult") else: print("Minor")` |
| `if-elif-else` | Checks multiple conditions | `if marks >= 90: print("A") elif marks >= 80: print("B") else: print("F")` |
| `Nested if` | `if` inside another `if` | `if age >= 18: if has_id: print("Allowed")` |
| **Ternary Operator** | Short-hand if-else | `status = "Adult" if age >= 18 else "Minor"` |
