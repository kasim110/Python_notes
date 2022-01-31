# Introduction🎃

Python is a cross-platform programming language, which means that it can run on multiple platforms like Windows, macOS, Linux, and 
has even been ported to the Java and .NET virtual machines. It is free and open-source.

Even though most of today's Linux and Mac have Python pre-installed in it, the version might be out-of-date.
So, it is always a good idea to install the most current version.

### Keywords
Keywords are the reserved words in Python.

We cannot use a keyword as a variable name, function name or any other identifier. They are used to define the syntax and structure of the Python language.

In Python, keywords are case sensitive.


|   `False`    |    `await`     |    `else`     |    `import`    |    `pass`    |
| :----------: | :------------: | :-----------: | :------------: | :----------: |
|  **`None`**  |  **`break`**   | **`except`**  |    **`in`**    | **`raise`**  |
|  **`True`**  |  **`class`**   | **`finally`** |    **`is`**    | **`return`** |
|  **`and`**   | **`continue`** |   **`for`**   |  **`lambda`**  |  **`try`**   |
|   **`as`**   |   **`def`**    |  **`from`**   | **`nonlocal`** | **`while`**  |
| **`assert`** |   **`del`**    | **`global`**  |   **`not`**    |  **`with`**  |
| **`async`**  |   **`elif`**   |   **`if`**    |    **`or`**    | **`yield`**  |

### Identifiers
An identifier is a name given to entities like class, functions, variables, etc. It helps to differentiate one entity from another.

1.Identifiers can be a combination of letters in lowercase **(a to z)** or uppercase **(A to Z)** or digits **(0 to 9)** or an underscore `_`. Names like `myClass`, `var_1` and `print_this_to_screen`, all are valid example.

2.An identifier cannot start with a digit. 1variable is invalid, but variable1 is a valid name.

3.Keywords cannot be used as identifiers.


```
global = 1
```
Output
```
File "<interactive input>", line 1
    global = 1
           ^
SyntaxError: invalid syntax
```
4.We cannot use special symbols like **!, @, #, $, %** etc. in our identifier.
```
a@ = 0
```
Output
```
File "<interactive input>", line 1
    a@ = 0
     ^
SyntaxError: invalid syntax
```
5.An identifier can be of any length.

### Things to Remember
Python is a case-sensitive language. This means, `Variable` and `variable` are not the same.

Always give the identifiers a name that makes sense. While `c = 10` is a valid name, writing `count = 10` would make more sense, and it would be easier to figure out what it represents when you look at your code after a long gap.

Multiple words can be separated using an underscore, like `this_is_a_long_variable`.

### Statement
```python
a = 10
# Multi line statement
a = 1 + 2 + 3 + \
    4 + 5 + 6 + \
    7 + 8 + 9

colors = ['red',
          'blue',
          'green']
# Multi statemets in single line
a = 1; b = 2; c = 3
```
### Comments
```python
#Single line comment

"""This is also a
perfect example of
multi-line comments"""
```
### Variables
A variable is a named location used to store data in the memory. It is helpful to think of variables as a container that holds data that can be changed later in the program.

You can think of variables as a bag to store books in it and that book can be replaced at any time.
```
number = 10
number = 1.1
```
Initially, the value of `number` was `10`. Later, it was changed to `1.1`.

**Note**: In Python, we don't actually assign values to the variables. Instead, Python gives the reference of the object(value) to the variable.

**Example**
```python
a, b, c = 5, 3.2, "Hello"

print (a)              # Output: 5
print (b)              # Output: 3.2
print (c)              # Output: Hello

# Assign same value to all variable
a, b, c = "same"

```

### Constants
A constant is a type of variable whose value cannot be changed. It is helpful to think of constants as containers that hold information which cannot be changed later.

### Assigning value to constant in Python

In Python, constants are usually declared and assigned in a module. Here, the module is a new file containing variables, functions, etc which is imported to the main file.
Inside the module, constants are written in all capital letters and underscores separating the words.

**Declaring and assigning value to a constant**

Create a **constant.py**:
```python
PI = 3.14
GRAVITY = 9.8
```
Create a **main.py**:
```python
import constant

print(constant.PI)
print(constant.GRAVITY)
```
**Output**
```
3.14
9.8
```

**📌 Note**: In reality, we don't use constants in Python. Naming them in all capital letters is a convention to separate them from variables, however, it does not actually prevent reassignment.
