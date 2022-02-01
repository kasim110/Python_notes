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

### Literals
Literal is a raw data given in a variable or constant. In Python, there are various types of literals they are as follows:
#### Numeric Literals
Numeric Literals are immutable (unchangeable). Numeric literals can belong to 3 different numerical types: `Integer`, `Float`, and `Complex`.

**How to use Numeric literals in Python?**
```python
a = 0b1010 #Binary Literals
b = 100 #Decimal Literal 
c = 0o310 #Octal Literal
d = 0x12c #Hexadecimal Literal

#Float Literal
float_1 = 10.5 
float_2 = 1.5e2

#Complex Literal 
x = 3.14j

print(a, b, c, d)
print(float_1, float_2)
print(x, x.imag, x.real)
```
**Output**
```python
10 100 200 300
10.5 150.0
3.14j 3.14 0.0
```

In the above program,

- We assigned integer literals into different variables. Here, `a` is binary literal, `b` is a decimal literal, `c` is an octal literal and `d` is a hexadecimal literal.
- When we print the variables, all the literals are converted into decimal values.
- `10.5` and `1.5e2` are floating-point literals. `1.5e2` is expressed with exponential and is equivalent to `1.5 * 102`.
- We assigned a complex literal i.e `3.14j` in variable `x`. Then we use imaginary literal (x.imag) and **real** literal (x.real) to create imaginary and real parts of complex numbers.

---------
#### String literals

A string literal is a sequence of characters surrounded by quotes. We can use both single, double, or triple quotes for a string. And, a character literal is a single character surrounded by single or double quotes.
**How to use string literals in Python?**

```
strings = "This is Python"
char = "C"
multiline_str = """This is a multiline string with more than one line code."""
unicode = u"\u00dcnic\u00f6de"
raw_str = r"raw \n string"

print(strings)
print(char)
print(multiline_str)
print(unicode)
print(raw_str)
```
**Output**

```
This is Python
C
This is a multiline string with more than one line code.
Ünicöde
raw \n string
```
In the above program, This is Python is a string literal and C is a character literal.

The value in triple-quotes `"""` assigned to the `multiline_str` is a multi-line string literal.

The string u"\u00dcnic\u00f6de" is a Unicode literal which supports characters other than English. In this case, \u00dc represents `Ü` and \u00f6 represents `ö`.

r"raw \n string" is a raw string literal.

------

#### Boolean literals

A Boolean literal can have any of the two values: `True` or `False`.
**How to use boolean literals in Python?**
```
x = (1 == True)
y = (1 == False)
a = True + 4
b = False + 10

print("x is", x)
print("y is", y)
print("a:", a)
print("b:", b)
```

**Output**
```
x is True
y is False
a: 5
b: 10
```

In the above program, we use boolean literal `True` and `False`. In Python, `True` represents the value as `1` and `False` as `0`. The value of `x` is `True` because `1` is equal to `True`. And, the value of `y` is `False` because `1` is not equal to `False`.

Similarly, we can use the `True` and `False` in numeric expressions as the value. The value of `a` is `5` because we add `True` which has a value of `1` with `4`. Similarly, `b` is `10` because we add the `False` having value of `0` with `10`.

------

#### Special literals
Python contains one special literal i.e. `None`. We use it to specify that the field has not been created.

**How to use special literals in Python?**
```
drink = "Available"
food = None

def menu(x):
    if x == drink:
        print(drink)
    else:
        print(food)

menu(drink)
menu(food)
```
**Output**
```
Available
None
```

In the above program, we define a `menu` function. Inside `menu`, when we set the argument as `drink` then, it displays `Available`. And, when the argument is `food`, it displays `None`.

-------

#### Literal Collections
There are four different literal collections List literals, Tuple literals, Dict literals, and Set literals.

**How to use literals collections in Python?**
```
fruits = ["apple", "mango", "orange"] #list
numbers = (1, 2, 3) #tuple
alphabets = {'a':'apple', 'b':'ball', 'c':'cat'} #dictionary
vowels = {'a', 'e', 'i' , 'o', 'u'} #set

print(fruits)
print(numbers)
print(alphabets)
print(vowels)
```

**Output**
```
['apple', 'mango', 'orange']
(1, 2, 3)
{'a': 'apple', 'b': 'ball', 'c': 'cat'}
{'e', 'a', 'o', 'i', 'u'}
```

In the above program, we created a list of `fruits`, a tuple of `numbers`, a dictionary `dict` having values with keys designated to each value and a set of `vowels`.

## Docstrings
A docstring is short for documentation string.

Python docstrings (documentation strings) are the string literals that appear right after the definition of a function, method, class, or module.




