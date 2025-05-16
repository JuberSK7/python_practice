# 🐍 50 Simple Python Programs for Absolute Beginners

# Python Questions & Answers

### 1. How to print “Hello World” in Python?
```python
print("Hello World")
```

### 2. How to print “Hello + Username” with the user’s name?
```python
usertext = input("What is your name? ")
print("Hello", usertext)
```

### 3. How to add 2 numbers entered by the user?
```python
num1 = input('Enter first number: ')
num2 = input('Enter second number: ')
sum = float(num1) + float(num2)
print('The sum of {0} and {1} is {2}'.format(num1, num2, sum))
```

### 4. How to find the average of 2 numbers?
```python
num1 = input('Enter first number: ')
num2 = input('Enter second number: ')
average = (int(num1) + int(num2)) / 2
print('Average: {0}'.format(average))
```

### 5. How to calculate the entered Visa and Final Grade Average?
```python
visagrade = input('Enter your visa grade: ')
finalgrade = input('Enter your final grade: ')
average = (float(visagrade) * 0.3) + (float(finalgrade) * 0.7)
print("Average: {0}".format(average))
```

### 6. How to find the average of 3 written grades?
```python
firstexam = input('Your first exam: ')
secondexam = input('Your second exam: ')
thirdexam = input('Your third exam: ')
average = (float(firstexam) + float(secondexam) + float(thirdexam)) / 3
print("Average: {0}".format(average))
```

### 7. How to show class pass status (PASSED / FAILED)?
```python
average = input('Enter average: ')
if int(average) >= 50:
    print("Passed")
else:
    print("Failed")
```

### 8. How to check if a number is odd or even?
```python
num = int(input("Enter a number: "))
if (num % 2) == 0:
    print("{0} is Even".format(num))
else:
    print("{0} is Odd".format(num))
```

### 9. How to check if a number is positive, negative, or zero?
```python
num = float(input("Enter a number: "))
if num > 0:
    print("Positive number")
elif num == 0:
    print("Zero")
else:
    print("Negative number")
```

### 10. How to calculate body mass index?
```python
print("Body Mass Index Calculation Program")
height = float(input("Enter height (m): "))
weight = int(input("Enter weight (kg): "))
index = weight / (height * height)

if index <= 18:
    print("\nUnderweight BMI: {}".format(index))
elif index <= 25:
    print("\nNormal BMI: {}".format(index))
elif index <= 30:
    print("\nOverweight BMI: {}".format(index))
else:
    print("\nObese BMI: {}".format(index))
```

### 11. Can the person get a driver's license based on their age?
```python
age = input('Enter age: ')
if int(age) < 18:
    print("Not eligible for a driver's license")
else:
    print("Eligible for a driver's license")
```

### 12. How to list numbers from 1 to 100?
```python
for i in range(1, 101):
    print(i)
```

### 13. How to list even numbers from 1 to 100?
```python
for i in range(1, 101):
    if i % 2 == 0:
        print(i)
```

### 14. How to list odd numbers from 1 to 100?
```python
for i in range(1, 101):
    if i % 2 != 0:
        print(i)
```

### 15. How to find numbers between 1 and 100 divisible by 3 or 5?
```python
for i in range(1, 101):
    if i % 3 == 0 or i % 5 == 0:
        print(i)
```

### 16. How to list numbers from 1 to a user-entered number?
```python
num = input('Enter number: ')
for i in range(1, int(num) + 1):
    print(i)
```

### 17. How to find the area and perimeter of a rectangle?
```python
short = input('Enter short side: ')
tall = input('Enter tall side: ')
area = int(short) * int(tall)
perimeter = 2 * (int(short) + int(tall))
print("Area: {0}".format(area))
print("Perimeter: {0}".format(perimeter))
```

### 18. How to print the letters of a word one per line?
```python
word = input("Enter a word: ")
for char in word:
    print(char)
```

### 19. How to find the sum of numbers between two numbers?
```python
sumofnumbers = 0
num1 = int(input('First number: '))
num2 = int(input('Second number: '))
for i in range(num1 + 1, num2):
    sumofnumbers += i
print("Sum of numbers between {0} and {1}: {2}".format(num1, num2, sumofnumbers))
```

### 20. Cinema or Theater Fee with Student Discount
```python
selection = input("Press (1) for Cinema, (2) for Theater: ")
student = input("Are you a student (Y/N)? ")
price = 0

if selection == '1':
    price = 10
elif selection == '2':
    price = 5

if student.lower() == 'y':
    price = price / 2

print("The fee you have to pay: {}".format(price))
```

### 21. How to check if a number is prime?
```python
num = int(input("Enter a number: "))
if num > 1:
    for i in range(2, num):
        if (num % i) == 0:
            print(num, "is not a prime number")
            break
    else:
        print(num, "is a prime number")
else:
    print(num, "is not a prime number")
```

### 22. Sum of odd and even numbers from user input
```python
NumList = []
Even_Sum = 0
Odd_Sum = 0

Number = int(input("Enter the total number of list elements: "))
for i in range(1, Number + 1):
    value = int(input("Enter value for element %d: " % i))
    NumList.append(value)

for j in range(Number):
    if NumList[j] % 2 == 0:
        Even_Sum += NumList[j]
    else:
        Odd_Sum += NumList[j]

print("Sum of even numbers =", Even_Sum)
print("Sum of odd numbers =", Odd_Sum)
```

### 23. Calculate increased salary based on raise rate
```python
salary = input("Enter current salary: ")
raise_rate = input("Salary raise rate (%): ")
new_salary = int(salary) + (int(salary) * int(raise_rate) / 100)
print("Increased salary:", new_salary)
```

### 24. Area and circumference of a circle using function
```python
import math

def find_Diameter(radius):
    return 2 * radius

def find_Circumference(radius):
    return 2 * math.pi * radius

def find_Area(radius):
    return math.pi * radius * radius

r = float(input('Enter the radius: '))
print("Diameter =", find_Diameter(r))
print("Circumference =", find_Circumference(r))
print("Area =", find_Area(r))
```

### 25. Area and perimeter of a rectangle using functions
```python
def areaRectangle(a, b):
    return a * b

def perimeterRectangle(a, b):
    return 2 * (a + b)

a = 5
b = 6
print("Area =", areaRectangle(a, b))
print("Perimeter =", perimeterRectangle(a, b))
```

### 26. Number guessing game
```python
import random
import math

lower = int(input("Enter lower bound: "))
upper = int(input("Enter upper bound: "))

x = random.randint(lower, upper)
chances = round(math.log(upper - lower + 1, 2))
print(f"You have {chances} chances to guess the number!")

count = 0
while count < chances:
    count += 1
    guess = int(input("Guess a number: "))

    if x == guess:
        print(f"Congratulations! You did it in {count} tries.")
        break
    elif x > guess:
        print("You guessed too low!")
    else:
        print("You guessed too high!")

if count >= chances and x != guess:
    print(f"The number was {x}. Better luck next time!")
```

### 27. What day of the week is a given date?
```python
import datetime

date = input('Enter a date (DD MM YYYY): ')
day_name = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
day = datetime.datetime.strptime(date, '%d %m %Y').weekday()
print(day_name[day])
```

### 28. Find missing numbers in a sorted list
```python
def find_missing(lst):
    return [x for x in range(lst[0], lst[-1] + 1) if x not in lst]

lst = [1, 2, 4, 6, 7, 9, 10]
print(find_missing(lst))
```

### 29. Check if a string contains specific characters
```python
char_list = ["a", "b", "c"]
string = "abcd"
matched_list = [char in char_list for char in string]
print(matched_list)

string_contains_chars = all(matched_list)
print(string_contains_chars)
```
---

### 32. How to insert records into a MySQL database on Python?

```python
import pymysql.cursors

connection = pymysql.connect(
    host='localhost',
    user='root',
    password='',
    db='students',
    charset='utf8mb4',
    cursorclass=pymysql.cursors.DictCursor
)

try:
    with connection.cursor() as cursor:
        sql = "INSERT INTO `users` (`firstname`, `lastname`) VALUES (%s, %s)"
        firstname = input("Enter first name: ")
        lastname = input("Enter last name: ")
        cursor.execute(sql, (firstname, lastname))
        connection.commit()
        print("User added successfully.")
finally:
    connection.close()
```

---

### 33. How to update records in a MySQL database on Python?

```python
import pymysql.cursors

connection = pymysql.connect(
    host='localhost',
    user='root',
    password='',
    db='students',
    charset='utf8mb4',
    cursorclass=pymysql.cursors.DictCursor
)

try:
    with connection.cursor() as cursor:
        user_id = input("Enter user ID to update: ")
        new_firstname = input("Enter new first name: ")
        sql = "UPDATE `users` SET `firstname` = %s WHERE `id` = %s"
        cursor.execute(sql, (new_firstname, user_id))
        connection.commit()
        print("Record updated successfully.")
finally:
    connection.close()
```

---

### 34. How to delete records from a MySQL database on Python?

```python
import pymysql.cursors

connection = pymysql.connect(
    host='localhost',
    user='root',
    password='',
    db='students',
    charset='utf8mb4',
    cursorclass=pymysql.cursors.DictCursor
)

try:
    with connection.cursor() as cursor:
        user_id = input("Enter user ID to delete: ")
        sql = "DELETE FROM `users` WHERE `id` = %s"
        cursor.execute(sql, (user_id,))
        connection.commit()
        print("User deleted successfully.")
finally:
    connection.close()
```

---

### 35. How to create a login form using Python and MySQL?

```python
import pymysql.cursors

connection = pymysql.connect(
    host='localhost',
    user='root',
    password='',
    db='students',
    charset='utf8mb4',
    cursorclass=pymysql.cursors.DictCursor
)

try:
    with connection.cursor() as cursor:
        username = input("Enter username: ")
        password = input("Enter password: ")
        sql = "SELECT * FROM `users` WHERE `username` = %s AND `password` = %s"
        cursor.execute(sql, (username, password))
        result = cursor.fetchone()
        if result:
            print("Login successful!")
        else:
            print("Invalid username or password.")
finally:
    connection.close()
```

---

### 36. How to create a Tkinter form with two input fields?

```python
import tkinter as tk

def show_data():
    print("Name:", name_entry.get())
    print("Age:", age_entry.get())

root = tk.Tk()
root.title("Simple Form")

tk.Label(root, text="Name:").grid(row=0, column=0)
tk.Label(root, text="Age:").grid(row=1, column=0)

name_entry = tk.Entry(root)
age_entry = tk.Entry(root)

name_entry.grid(row=0, column=1)
age_entry.grid(row=1, column=1)

submit_btn = tk.Button(root, text="Submit", command=show_data)
submit_btn.grid(row=2, column=1)

root.mainloop()
```

---

### 37. How to create a list of squares using a list comprehension?

```python
squares = [x ** 2 for x in range(1, 11)]
print("Squares from 1 to 10:", squares)
```

---

### 38. How to check if a string is a palindrome in Python?

```python
def is_palindrome(s):
    return s == s[::-1]

string = input("Enter a string: ")
if is_palindrome(string):
    print("It's a palindrome.")
else:
    print("It's not a palindrome.")
```

---

### 39. How to find the factorial of a number using recursion?

```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)

num = int(input("Enter a number: "))
print(f"Factorial of {num} is {factorial(num)}")
```

---

### 40. How to use `try` and `except` blocks in Python?

```python
try:
    num = int(input("Enter a number: "))
    result = 10 / num
    print("Result:", result)
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Invalid input! Please enter a number.")
```

---

### 41. How to generate a random password in Python?

```python
import random
import string

def generate_password(length=8):
    chars = string.ascii_letters + string.digits + string.punctuation
    return ''.join(random.choice(chars) for _ in range(length))

print("Generated password:", generate_password(12))
```

---

### 42. How to count vowels in a string in Python?

```python
def count_vowels(s):
    return sum(1 for char in s.lower() if char in "aeiou")

text = input("Enter text: ")
print("Number of vowels:", count_vowels(text))
```

---

### 43. How to reverse words in a sentence?

```python
sentence = input("Enter a sentence: ")
words = sentence.split()
reversed_sentence = ' '.join(reversed(words))
print("Reversed sentence:", reversed_sentence)
```

---

### 44. How to merge two dictionaries in Python?

```python
dict1 = {'a': 1, 'b': 2}
dict2 = {'b': 3, 'c': 4}
merged = {**dict1, **dict2}
print("Merged dictionary:", merged)
```

---

### 45. How to remove duplicates from a list in Python?

```python
my_list = [1, 2, 2, 3, 4, 4, 5]
unique_list = list(set(my_list))
print("Unique list:", unique_list)
```

---

### 46. How to find the largest number in a list?

```python
numbers = [10, 45, 32, 67, 2]
print("Largest number is:", max(numbers))
```

---

### 47. How to find the second largest number in a list?

```python
numbers = [10, 45, 32, 67, 2]
unique_numbers = list(set(numbers))
unique_numbers.sort()
print("Second largest number is:", unique_numbers[-2])
```

---

### 48. How to read a text file line by line in Python?

```python
with open("sample.txt", "r") as file:
    for line in file:
        print(line.strip())
```

---

### 49. How to write user input to a text file?

```python
with open("output.txt", "w") as file:
    text = input("Enter something to write to the file: ")
    file.write(text)
    print("Text written to output.txt")
```

---

### 50. How to create a basic calculator using functions?

```python
def add(x, y): return x + y
def subtract(x, y): return x - y
def multiply(x, y): return x * y
def divide(x, y): return x / y if y != 0 else "Cannot divide by zero"

print("Options: +, -, *, /")
a = float(input("Enter first number: "))
op = input("Enter operator: ")
b = float(input("Enter second number: "))

if op == '+':
    print("Result:", add(a, b))
elif op == '-':
    print("Result:", subtract(a, b))
elif op == '*':
    print("Result:", multiply(a, b))
elif op == '/':
    print("Result:", divide(a, b))
else:
    print("Invalid operator.")
```



