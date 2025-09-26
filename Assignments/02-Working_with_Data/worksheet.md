# 📝 Worksheet: 02 - Working with Data


---

## 🧠 Section 1: Lists

1. What method adds an item to the end of a list?  
   `Answer: .append()`

2. How can you remove an item from a list by value?  
   `Answer: .remove(value)`

3. What’s the result of this code?

```python
nums = [2, 4, 6]
nums.append(8)
print(nums)
```

   `Answer:[2, 4, 6, 8]` 

---

### ✏️ Task: List Practice

```python
# Create a list of your top 3 favorite foods.
# Add another food to the list.
# Remove one item and print the list.

# Input 3 favorite food
foods = []
for i in range(3):
    item = input(f"Enter your favourite food {i+1}: ")
    foods.append(item)

# Print current list
print("List of your favorite food:", foods)

# Add 1 new food in the list
new_food = input("Enter another food: ")
foods.append(new_food)

# Print new list
print("List after you add another food:", foods)

# Delete 1 food in th list
remove_food = input("Enter the food you want to delete: ")
if remove_food in foods:
    foods.remove(remove_food)
else:
    print(f"{remove_food} not in the list!")

# Print finally lists
print("This is your finally list:", foods)

Enter your favourite food 1: Pizza
Enter your favourite food 2: Burger
Enter your favourite food 3: Pasta
List of your favorite food: ['Pizza', 'Burger', 'Pasta']
Enter another food: Noodle
List after you add another food: ['Pizza', 'Burger', 'Pasta', 'Noodle']
Enter the food you want to delete: Pasta
This is your finally list: ['Pizza', 'Burger', 'Noodle']
```

---

## 🔒 Section 2: Tuples

4. What is a key difference between a list and a tuple?  
   `Answer: .append()`

5. Can you change the contents of a tuple once it is created? Why or why not?  
   `Answer: .remove(value)` 

---

### ✏️ Task: Tuple Practice

```python
# Create a tuple with your favorite 3 numbers.
# Unpack it into three variables and print each.

# Enter 3 number
a = int(input("Your favorites number 1: "))
b = int(input("Your favorites number 2: "))
c = int(input("Your favorites number 3: "))

numbers = (a, b, c)

# Print Tuple
print("Tuple is :", numbers)

# Unpack and print each number
x, y, z = numbers
print("Number 1:", x)
print("Number 2:", y)
print("Number 3:", z)

Your favorites number 1: 6
Your favorites number 2: 9
Your favorites number 3: 12
Tuple is : (6, 9, 12)
Number 1: 6
Number 2: 9
Number 3: 12
```

---

## 🔑 Section 3: Dictionaries

6. What does the `.get()` method do differently from accessing a key directly?  
   `Answer: .get() returns None (or a default value you specify) if the key is missing, instead of causing an error.` 

7. How do you loop through both keys and values in a dictionary?  
   `Answer: Use .items() in a for loop → for key, value in dict.items():` 

---

### ✏️ Task: Dictionary Practice

```python
# Create a dictionary with keys: 'name', 'age', and 'hobby'.
# Print each key and value in the format "key: value".

# Enter your information 
name = input("Enter your name: ")
age = int(input("Enter your age: "))
fav_color = input("Enter your favorite color: ")

# Your info
info = (name, age, fav_color)

# Print your info
print("Your information:", info)

Enter your name: Riley
Enter your age: 22
Enter your favorite color: RED
Your information: ('Riley', 22, 'RED')
```

---

## 🧾 Submit Checklist

- [ ] I practiced creating and modifying lists.
- [ ] I understand how tuples are different from lists.
- [ ] I accessed and looped through dictionary items.
