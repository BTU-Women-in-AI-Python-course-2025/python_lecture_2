# **Loops in Python**
Loops are used in Python to **execute a block of code multiple times**. Python provides two types of loops:

1. **for loop** – Used to iterate over a sequence (list, tuple, dictionary, string, etc.).
2. **while loop** – Repeats a block of code as long as a condition is `True`.

We also have **loop control statements**:
- `break` – Exits the loop immediately.
- `continue` – Skips the current iteration and moves to the next.

---

## **1. for Loop**
The `for` loop is used to iterate over a sequence like a list, tuple, string, or range.

### **Syntax:**
```python
for variable in sequence:
    # Code to execute in each iteration
```

### **Example 1: Iterating Over a List**
```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)
```
**Output:**
```
apple
banana
cherry
```

---

### **Example 2: Using `range()` in a for loop**
The `range(start, stop, step)` function generates a sequence of numbers.

```python
for i in range(1, 6):  # Loops from 1 to 5
    print(i)
```
**Output:**
```
1
2
3
4
5
```

---

### **Example 3: Iterating Over a String**
```python
for letter in "Python":
    print(letter)
```
**Output:**
```
P
y
t
h
o
n
```

---

## **2. while Loop**
The `while` loop continues executing as long as the condition is `True`.

### **Syntax:**
```python
while condition:
    # Code to execute
```

### **Example 1: Printing numbers from 1 to 5**
```python
x = 1

while x <= 5:
    print(x)
    x += 1  # Increment x
```
**Output:**
```
1
2
3
4
5
```

---

### **Example 2: Using `while` to ask for user input**
```python
password = ""

while password != "1234":
    password = input("Enter password: ")

print("Access granted!")
```
This keeps asking for the password **until** the user enters `"1234"`.

---

## **3. break Statement**
The `break` statement **exits the loop immediately**.

### **Example: Stopping a loop when a condition is met**
```python
for num in range(1, 10):
    if num == 5:
        break  # Loop stops when num is 5
    print(num)
```
**Output:**
```
1
2
3
4
```

---

## **4. continue Statement**
The `continue` statement **skips the current iteration** and moves to the next.

### **Example: Skipping even numbers**
```python
for num in range(1, 6):
    if num % 2 == 0:
        continue  # Skips even numbers
    print(num)
```
**Output:**
```
1
3
5
```

---

## **Summary Table**
| Loop Type | Description | Example |
|-----------|-------------|---------|
| `for` loop | Iterates over a sequence | `for x in range(5): print(x)` |
| `while` loop | Runs while a condition is `True` | `while x < 5: print(x); x+=1` |
| `break` | Exits the loop | `for x in range(5): if x == 3: break` |
| `continue` | Skips current iteration | `for x in range(5): if x == 3: continue` |
