# Milestone solution for python modules

by Dorcas T Mutyavaviri
**Why Python Programming is Awesome:**
Python is a versatile, high-level programming language known for its simplicity, readability, and vast community support. Its clean and concise syntax makes it easy to learn and write code quickly. Python boasts a rich standard library and a massive ecosystem of third-party packages, making it suitable for a wide range of applications such as web development, data analysis, scientific computing, machine learning, and more. Its interpreted nature allows for rapid development and testing, and it's cross-platform, running seamlessly on various operating systems.

**How to Import Functions from Another File:**
You can import functions from another file using the `import` statement. Suppose you have a file named `my_module.py` containing a function called `my_function`:

```python
# my_module.py
def my_function():
    return "Hello from my_function!"
```

In another file, you can import and use this function like this:

```python
import my_module

result = my_module.my_function()
print(result)
```

**How to Create a Module:**
A module in Python is a file containing Python definitions and statements. To create a module, simply write your code in a `.py` file. For instance, let's say you have a file named `math_operations.py`:

```python
# math_operations.py
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b
```

You can then import and use these functions in another file:

```python
import math_operations

sum_result = math_operations.add(5, 3)
print(sum_result)
```

**How to Use the Built-in Function `dir()`:**
The `dir()` function returns a list of names in the current local scope or the attributes of an object if an object is passed as an argument. It's commonly used for introspection and exploring available attributes of modules, objects, or classes.

Example with modules:

```python
import math
print(dir(math))
```

Example with objects:

```python
my_list = [1, 2, 3]
print(dir(my_list))
```

**How to Prevent Code from Being Executed When Imported:**
To prevent code from being executed when a script is imported as a module, you can use the `if __name__ == '__main__':` idiom. This ensures that the code block under this condition only runs if the script is executed directly and not when imported.

```python
def my_function():
    return "Hello from my_function!"

if __name__ == '__main__':
    result = my_function()
    print(result)
```

**How to Use Command Line Arguments with Your Python Programs:**
You can use the `sys` module to access command line arguments in your Python script. Here's a basic example:

```python
import sys

if len(sys.argv) > 1:
    argument = sys.argv[1]
    print("You provided an argument:", argument)
else:
    print("No arguments provided.")
```

If you run this script from the command line with `python script.py hello`, it will output: "You provided an argument: hello".
