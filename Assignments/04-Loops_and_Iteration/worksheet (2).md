# 📝 Worksheet: 04 - Loops and Iteration

Practice and reflect on how loops work in Python.

---

## 🔁 Section 1: For Loops

1. What does `range(5)` produce?

`Answer: 0, 1, 2, 3, 4` 

2. Write a `for` loop that prints numbers 1 to 10, but skips 5.

```python
# Your code:
for i in range (1, 11):
  if i == 5:
    continue
  print(i)

1
2
3
4
6
7
8
9
10
```

---

## 🔁 Section 2: While Loops

3. What’s the difference between a `for` loop and a `while` loop?

`Answer: A "for" loop is a loop predetermined number of times (or through each element in a sequence), while a "while" loop is a continuous loop as long as the condition is true.
`

4. What happens if a `while` loop's condition never becomes `False`?

`Answer: It creates an infinite loop, and a program will never pause.` 

---

### ✏️ Task: Countdown with While

```python
# Use a while loop to count down from 5 to 1.

count = 5
while count >= 1:
    print(count)
   count -= 1

5
4
3
2
1
```

---

## 📁 Section 3: File Reading and `with`

5. What does the `with` statement do when opening a file?

`Answer: with automatically closes the file after the inner block of code completes, helping to avoid errors and resource leaks.`

6. How do you loop over each line in a file?
`Answer: for line in file: `
---

### ✏️ Task: File Filter

Write code that prints only the lines in a file that contain the word `"error"`.

```python
# Your code here
with open('log.txt', 'r') as file:
    for line in file:
        if 'error' in line.lower():
            print(line.strip())
```
