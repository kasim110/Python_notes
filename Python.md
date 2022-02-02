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

Python docstrings (documentation strings) are the [string](https://www.programiz.com/python-programming/string) literals that appear right after the definition of a function, method, class, or module.

**Example**
```python
def double(num):
    """Function to double the value"""
    return 2*num
    print(double.__doc__)
```
**Output**
```
Function to double the value
```

**Docstrings for the built-in-function**
```python
print(print.__doc__)
```
**Output**
```
print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)

Prints the values to a stream, or to sys.stdout by default.
Optional keyword arguments:
file:  a file-like object (stream); defaults to the current sys.stdout.
sep:   string inserted between values, default a space.
end:   string appended after the last value, default a newline.
flush: whether to forcibly flush the stream.
```

## Data types

```python
a = 5
print(a, "is of type", type(a))

a = 2.0
print(a, "is of type", type(a))

a = 1+2j
print(a, "is complex number?", isinstance(1+2j,complex))
```

**Output**
```
5 is of type <class 'int'>
2.0 is of type <class 'float'>
(1+2j) is complex number? True
```

### List
`List` is an ordered sequence of items. It is one of the most used datatype in Python and is very flexible. All the items in a list do not need to be of the same type.

Declaring a list is pretty straight forward. Items separated by commas are enclosed within brackets `[ ]`.

```python
a = [5,10,15,20,25,30,35,40]

# a[2] = 15
print("a[2] = ", a[2])

# a[0:3] = [5, 10, 15]
print("a[0:3] = ", a[0:3])

# a[5:] = [30, 35, 40]
print("a[5:] = ", a[5:])
```

#### **Create list**

```python
# empty list
my_list = []

# list of integers
my_list = [1, 2, 3]

# list with mixed data types
my_list = [1, "Hello", 3.4]

# nested list
my_list = ["mouse", [8, 4, 6], ['a']]
```
#### **Access elements from list**

```python
# List indexing

my_list = ['p', 'r', 'o', 'b', 'e']

# Output: p
print(my_list[0])

# Output: o
print(my_list[2])

# Output: e
print(my_list[4])

# Nested List 
n_list = ["Happy", [2, 0, 1, 5]]

# Nested indexing
# Output: a
print(n_list[0][1])
# Output: 5
print(n_list[1][3])

# Error! Only integer can be used for indexing
print(my_list[4.0])
```
#### Negative indexing

Python allows negative indexing for its sequences. The index of -1 refers to the last item, -2 to the second last item and so on.

```python
# Negative indexing in lists
my_list = ['p','r','o','b','e']

print(my_list[-1])

print(my_list[-5])
```

When we run the above program, we will get the following output:

```
e
p
```

#### Slice lists in Python

We can access a range of items in a list by using the slicing operator `:`(colon).

```python
# List slicing in Python

my_list = ['p','r','o','g','r','a','m','i','z']

# elements 3rd to 5th
print(my_list[2:5])

# elements beginning to 4th
print(my_list[:-5])

# elements 6th to end
print(my_list[5:])

# elements beginning to end
print(my_list[:])
```
**Output**

```
['o', 'g', 'r']
['p', 'r', 'o', 'g']
['a', 'm', 'i', 'z']
['p', 'r', 'o', 'g', 'r', 'a', 'm', 'i', 'z']
```

Slicing can be best visualized by considering the index to be between the elements as shown below. So if we want to access a range, we need two indices that will slice that portion from the list.

#### How to change elements to a list?

Lists are mutable, meaning their elements can be changed unlike [string](https://www.programiz.com/python-programming/string) or [tuple](https://www.programiz.com/python-programming/tuple).

We can use the assignment operator (`=`) to change an item or a range of items.

```python
# Correcting mistake values in a list
odd = [2, 4, 6, 8]

# change the 1st item    
odd[0] = 1            

print(odd)

# change 2nd to 4th items
odd[1:4] = [3, 5, 7]  

print(odd)                   
```

**Output**

```
[1, 4, 6, 8]
[1, 3, 5, 7]
```

#### Add Elements

```python
odd = [1, 3, 5]
# add one item
odd.append(7)

print(odd)

# add several items using extend
odd.extend([9, 11, 13])

print(odd)

even = [2, 4, 6, 8]
print(even + [10, 12, 14])

print(["re"] * 3)


```

**Output**

```
[1, 3, 5, 7]
[1, 3, 5, 7, 9, 11, 13]
[2, 4, 6, 8, 10, 12, 14]
['re', 're', 're']
```

#### List Methods

| [Python List Methods](https://www.programiz.com/python-programming/methods/list) |
| :----------------------------------------------------------- |
| [**append() -**](https://www.programiz.com/python-programming/methods/list/append) [Add an element to the end of the list](https://www.programiz.com/python-programming/methods/list/append) |
| [**extend()**](https://www.programiz.com/python-programming/methods/list/extend) [-](https://www.programiz.com/python-programming/methods/list/extend) [Add all elements of a list to the another list](https://www.programiz.com/python-programming/methods/list/extend) |
| [**insert()**](https://www.programiz.com/python-programming/methods/list/insert) [-](https://www.programiz.com/python-programming/methods/list/insert) [Insert an item at the defined index](https://www.programiz.com/python-programming/methods/list/insert) |
| [**remove()**](https://www.programiz.com/python-programming/methods/list/remove) [-](https://www.programiz.com/python-programming/methods/list/remove) [Removes an item from the list](https://www.programiz.com/python-programming/methods/list/remove) |
| [**pop()**](https://www.programiz.com/python-programming/methods/list/pop) [-](https://www.programiz.com/python-programming/methods/list/pop) [Removes and returns an element at the given index](https://www.programiz.com/python-programming/methods/list/pop) |
| [**clear()**](https://www.programiz.com/python-programming/methods/list/clear) [- Removes all items from the list](https://www.programiz.com/python-programming/methods/list/clear) |
| [**index()**](https://www.programiz.com/python-programming/methods/list/index) [- Returns the index of the first matched item](https://www.programiz.com/python-programming/methods/list/index) |
| [**count()**](https://www.programiz.com/python-programming/methods/list/count) [- Returns the count of the number of items passed as an argument](https://www.programiz.com/python-programming/methods/list/count) |
| [**sort()**](https://www.programiz.com/python-programming/methods/list/sort) [- Sort items in a list in ascending order](https://www.programiz.com/python-programming/methods/list/sort) |
| [**reverse()**](https://www.programiz.com/python-programming/methods/list/reverse) [- Reverse the order of items in the list](https://www.programiz.com/python-programming/methods/list/reverse) |
| [**copy()**](https://www.programiz.com/python-programming/methods/list/copy) [- R](https://www.programiz.com/python-programming/methods/list/copy)[eturns a shallow copy of the list](https://www.programiz.com/python-programming/methods/list/copy) |
| **len()** [-] Length of string                                        |

```python
# Output: [1, 2, 4, 8, 16, 32, 64, 128, 256, 512]
pow2 = [2 ** x for x in range(10)]
print(pow2)
```

### Tuple
[Tuple](https://www.programiz.com/python-programming/tuple) is an ordered sequence of items same as a list. The only difference is that tuples are immutable. Tuples once created cannot be modified.

Tuples are used to write-protect data and are usually faster than lists as they cannot change dynamically.

It is defined within parentheses `()` where items are separated by commas.

```python
# Different types of tuples

# Empty tuple
my_tuple = ()
print(my_tuple)

# Tuple having integers
my_tuple = (1, 2, 3)
print(my_tuple)

# tuple with mixed datatypes
my_tuple = (1, "Hello", 3.4)
print(my_tuple)

# nested tuple
my_tuple = ("mouse", [8, 4, 6], (1, 2, 3))
print(my_tuple)
```
**Output**
```
()
(1, 2, 3)
(1, 'Hello', 3.4)
('mouse', [8, 4, 6], (1, 2, 3))
```

#### Advantages of Tuple over List
Since tuples are quite similar to lists, both of them are used in similar situations. However, there are certain advantages of implementing a tuple over a list. Below listed are some of the main advantages:

- We generally use tuples for heterogeneous (different) data types and lists for homogeneous (similar) data types.
- Since tuples are immutable, iterating through a tuple is faster than with list. So there is a slight performance boost.
- Tuples that contain immutable elements can be used as a key for a dictionary. With lists, this is not possible.
- If you have data that doesn't change, implementing it as tuple will guarantee that it remains write-protected.

