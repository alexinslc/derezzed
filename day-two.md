## 🐍 Python Initialization

- [ ] Check to see if Python is installed: `python3 --version`
- [ ] If not, install it: `sudo apt install python3`
- [ ] Set up your project folder and move to it `mkdir -p ~/derezzed/day-two && cd ~/derezzed/day-two`

## 🐍 Python Basics

* Python is a high-level programming language that is easy to learn and widely used. It is used for web development, data analysis, artificial intelligence, scientific computing, and more. (insert link to good video)

### 👋 Welcome to The Grid
- [ ] Create a new file called `main.py` in your `day-two` directory.
- [ ] Open the file using `code .` and type in the following code:
```python
print("Welcome to The Grid!")
```
- [ ] Save the file and run it using `python3 main.py`

### 📦 Variables

* Variables are used to store data. In Python, creating a variable is simple. 

- [ ] Add the following code to the end your `main.py` file:

```python
# Create 2 variables one for lightcycle color and one for lightcycle speed
lightcycle_color = "blue"
lightcycle_speed = 20

# Print the variables
print("Lightcycle Color:", lightcycle_color)
print("Lightcycle Speed:", lightcycle_speed)
```

- [ ] Save the file and run it using `python3 main.py`

### ⚙️ Functions

* Fuctions are used to group code together. They can take inputs (called parameters) and return outputs.

- [ ] Add the following code to the end of your `main.py` file:

```python
def lightcycle_speed(speed):
    return speed * 2
def lightcycle_color(color):
    return color.upper()

# call the functions
print("Lightcycle Speed:", lightcycle_speed(20))
print("Lightcycle Color:", lightcycle_color("blue"))
```
- [ ] Save the file and run it using `python3 main.py`


### 🌐 Scope
* Scope refers to the visibility of variables in different parts of your code. Variables defined inside a function are not accessible outside of it.

- [ ] Add the following code to the end your `main.py` file:

```python
tron = "program"

def identity():
  print(tron)
```
- [ ] Save the file and run it using `python3 main.py`




### Data Types
* Python has several built-in data types. The most common ones are:
  - `int` (integer)
  - `float` (floating point number)
  - `str` (string)
  - `bool` (boolean)
  - `list` (list)
  - `tuple` (tuple)
  - `dict` (dictionary)
  - `set` (set)

- [ ] Add the following code to the end your `main.py` file:

```python
# Create a variable for each data type
lightcycle_color = "blue" # str
lightcycle_speed = 20 # int
lightcycle_speed_float = 20.5 # float
lightcycle_active = True # bool
lightcycle_colors = ["blue", "red", "green"] # list
lightcycle_colors_tuple = ("blue", "red", "green") # tuple
lightcycle_colors_dict = {"blue": "lightcycle", "red": "lightcycle"} # dict
lightcycle_colors_set = {"blue", "red", "green"} # set
# Print the variables
print("Lightcycle Color:", lightcycle_color)
print("Lightcycle Speed:", lightcycle_speed)
print("Lightcycle Speed Float:", lightcycle_speed_float)
print("Lightcycle Active:", lightcycle_active)
print("Lightcycle Colors:", lightcycle_colors)
print("Lightcycle Colors Tuple:", lightcycle_colors_tuple)
print("Lightcycle Colors Dict:", lightcycle_colors_dict)
print("Lightcycle Colors Set:", lightcycle_colors_set)
```
- [ ] Save the file and run it using `python3 main.py`

### ➡️ Comparisons

* Comparisons are used to compare two values. The most common comparisons are:
  - `==` (equal to)
  - `!=` (not equal to)
  - `>` (greater than)
  - `<` (less than)
  - `>=` (greater than or equal to)
  - `<=` (less than or equal to)
* Comparisons return a boolean value (`True` or `False`).
* Comparisons can be used in `if` statements to control the flow of your code.

- [ ] Add the following code to the end your `main.py` file:

```python
# Create a variable for each comparison
lightcycle_color = "blue"

if lightcycle_color == "blue":
    print("Lightcycle is blue")
else:
    print("Lightcycle is not blue")
```
- [ ] Save the file and run it using `python3 main.py`

### Lists

* Lists are used to store multiple values in a single variable. They are ordered, changeable, and allow duplicate values.
* Lists are created using square brackets `[]` and can contain any data type.
* Lists can be accessed using their index (starting at 0) and can be modified using various methods.

- [ ] Add the following code to the end your `main.py` file:

```python
# Create a list of lightcycle colors
lightcycle_colors = ["blue", "red", "green"]
# Print the list
print("Lightcycle Colors:", lightcycle_colors)
# Add a color to the list
lightcycle_colors.append("yellow")
# Print the updated list
print("Updated Lightcycle Colors:", lightcycle_colors)
# Remove a color from the list
lightcycle_colors.remove("red")
# Print the updated list
print("Updated Lightcycle Colors:", lightcycle_colors)
# Access a color from the list
print("First Lightcycle Color:", lightcycle_colors[0])
```
- [ ] Save the file and run it using `python3 main.py`


### 🍭 Loops

* Loops are used to repeat a block of code multiple times. The most common loops are:
  - `for` loop
  - `while` loop

* Loops can be used to iterate over a list, tuple, or dictionary.
* Loops can also be used to repeat a block of code until a certain condition is met.

- [ ] Add the following code to the end your `main.py` file:

```python
# Create a list of lightcycle colors
lightcycle_colors = ["blue", "red", "green"]
# Iterate over the list and print each color
for color in lightcycle_colors:
    print("Lightcycle Color:", color)
```
- [ ] Save the file and run it using `python3 main.py`

### 📚 Dictionaries

* Dictionaries are used to store data values in key:value pairs. They are unordered, changeable, and do not allow duplicates.
* Dictionaries are created using curly braces `{}` and can contain any data type.
* Dictionaries can be accessed using their keys and can be modified using various methods.

- [ ] Add the following code to the end your `main.py` file:

```python
# Create a dictionary of lightcycle colors
lightcycle_colors = {
    "blue": "lightcycle",
    "red": "lightcycle",
    "green": "lightcycle"
}
# Print the dictionary
print("Lightcycle Colors:", lightcycle_colors)
# Add a color to the dictionary
lightcycle_colors["yellow"] = "lightcycle"
# Print the updated dictionary
print("Updated Lightcycle Colors:", lightcycle_colors)
# Remove a color from the dictionary
del lightcycle_colors["red"]
# Print the updated dictionary
print("Updated Lightcycle Colors:", lightcycle_colors)
# Access a color from the dictionary
print("Lightcycle Color:", lightcycle_colors["blue"])
```
- [ ] Save the file and run it using `python3 main.py`

### 🗝️ Sets

* Sets are used to store multiple values in a single variable. They are unordered, unchangeable, and do not allow duplicates.
* Sets are created using curly braces `{}` and can contain any data type.
* Sets can be accessed using their index (starting at 0) and can be modified using various methods.

- [ ] Add the following code to the end your `main.py` file:

```python
# Create a set of lightcycle colors
lightcycle_colors = {"blue", "red", "green"}
# Print the set
print("Lightcycle Colors:", lightcycle_colors)
# Add a color to the set
lightcycle_colors.add("yellow")
# Print the updated set
print("Updated Lightcycle Colors:", lightcycle_colors)
# Remove a color from the set
lightcycle_colors.remove("red")
# Print the updated set
print("Updated Lightcycle Colors:", lightcycle_colors)
# Access a color from the set
print("First Lightcycle Color:", list(lightcycle_colors)[0])
```
- [ ] Save the file and run it using `python3 main.py`

### ⚠️ Errors

* Errors are used to indicate that something went wrong in your code. The most common errors are:
  - `SyntaxError` (syntax error)
  - `NameError` (name error)
  - `TypeError` (type error)
  - `IndexError` (index error)
  - `KeyError` (key error)
* Errors can be handled using `try` and `except` statements.

- [ ] Add the following code to the end your `main.py` file:

```python 
try:
  print(1 / 0)
  except ZeroDivisionError:
  print("You can't divide by zero!")
```
- [ ] Save the file and run it using `python3 main.py`

### 🎯 Practice

