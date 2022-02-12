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
| **len()** - Length of string                                        |

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

### Strings
[String](https://www.programiz.com/python-programming/string) is sequence of Unicode characters. We can use single quotes or double quotes to represent strings. Multi-line strings can be denoted using triple quotes, `'''` or `"""`.

##### Access characters in a string
```python
#Accessing string characters in Python
str = 'programiz'
print('str = ', str)

#first character
print('str[0] = ', str[0])

#last character
print('str[-1] = ', str[-1])

#slicing 2nd to 5th character
print('str[1:5] = ', str[1:5])

#slicing 6th to 2nd last character
print('str[5:-2] = ', str[5:-2])
```
**Output**
```
str =  programiz
str[0] =  p
str[-1] =  z
str[1:5] =  rogr
str[5:-2] =  am
```
##### Iterating Through a string

```python
# Iterating through a string
count = 0
for letter in 'Hello World':
    if(letter == 'l'):
        count += 1
print(count,'letters found')
```
**Output**
```
3 letters found
```

##### String Membership Test
We can test if a substring exists within a string or not, using the keyword `in`.
```
>>> 'a' in 'program'
True
>>> 'at' not in 'battle'
False
```

Here is a list of all the **escape sequences** supported by Python.

| Escape Sequence  |  Description                         |
| :----------------|  :-----------------------------------|
| \newline	       |  Backslash and newline ignored       |
| \\	           |  Backslash                           |
| \'	           |  Single quote                        |
| \"	           |  Double quote                        |
| \a	           |  ASCII Bell                          |
| \b	           |  ASCII Backspace                     |
| \f               |  ASCII Formfeed                      |
| \n	           |  ASCII Linefeed                      |
| \r	           |  ASCII Carriage Return               |
| \t	           |  ASCII Horizontal Tab                |
| \v	           |  ASCII Vertical Tab                  |
| \ooo	           |  Character with octal value ooo      |
| \xHH	           |  Character with hexadecimal value HH |

**Note:** There are many string build in operations we can do.

### Set
A set is an unordered collection of items. Every set element is unique (no duplicates) and must be immutable (cannot be changed).
 
 However, a set itself is mutable. We can add or remove items from it.
 
 Sets can also be used to perform mathematical set operations like union, intersection, symmetric difference, etc.
 
 ##### Creating Sets
 A `set` is created by placing all the items (elements) inside curly braces `{}`, separated by comma, or by using the built-in `set()` function.
 
 ```python
 # Different types of sets in Python
# set of integers
my_set = {1, 2, 3}
print(my_set)

# set of mixed datatypes
my_set = {1.0, "Hello", (1, 2, 3)}
print(my_set)

# Distinguish set and dictionary while creating empty set

# initialize a with {}
a = {}

# check data type of a
print(type(a))

# initialize a with set()
a = set()

# check data type of a
print(type(a))
```
**Output**
```
{1, 2, 3}
{1.0, (1, 2, 3), 'Hello'}
```

##### Modifying a set in Python
Sets are mutable. However, since they are unordered, indexing has no meaning.

We cannot access or change an element of a set using indexing or slicing. Set data type does not support it.

We can add a single element using the `add()` method, and multiple elements using the `update()` method. The `update()` method can take [tuples](https://www.programiz.com/python-programming/tuple), lists,[strings](https://www.programiz.com/python-programming/string)  or other sets as its argument. In all cases, duplicates are avoided.

```python
# initialize my_set
my_set = {1, 3}
print(my_set)

# my_set[0]
# if you uncomment the above line
# you will get an error
# TypeError: 'set' object does not support indexing

# add an element
# Output: {1, 2, 3}
my_set.add(2)
print(my_set)

# add multiple elements
# Output: {1, 2, 3, 4}
my_set.update([2, 3, 4])
print(my_set)

# add list and set
# Output: {1, 2, 3, 4, 5, 6, 8}
my_set.update([4, 5], {1, 6, 8})
print(my_set)
```

**Output**
```
{1, 3}
{1, 2, 3}
{1, 2, 3, 4}
{1, 2, 3, 4, 5, 6, 8}
```

##### Removing elements from a set

A particular item can be removed from a set using the methods `discard()` and `remove()`.

The only difference between the two is that the `discard()` function leaves a set unchanged if the element is not present in the set. On the other hand, the `remove()` function will raise an error in such a condition (if element is not present in the set).

The following example will illustrate this.
```python
# Difference between discard() and remove()

# initialize my_set
my_set = {1, 3, 4, 5, 6}
print(my_set)

# discard an element
# Output: {1, 3, 5, 6}
my_set.discard(4)
print(my_set)

# remove an element
# Output: {1, 3, 5}
my_set.remove(6)
print(my_set)

# discard an element
# not present in my_set
# Output: {1, 3, 5}
my_set.discard(2)
print(my_set)

# remove an element
# not present in my_set
# you will get an error.
# Output: KeyError

my_set.remove(2)
```

**Output**
```
{1, 3, 4, 5, 6}
{1, 3, 5, 6}
{1, 3, 5}
{1, 3, 5}
Traceback (most recent call last):
  File "<string>", line 28, in <module>
KeyError: 2
```

Similarly, we can remove and return an item using the `pop()` method.

Since set is an unordered data type, there is no way of determining which item will be popped. It is completely arbitrary.

We can also remove all the items from a set using the `clear()` method.

```python
# initialize my_set
# Output: set of unique elements
my_set = set("HelloWorld")
print(my_set)

# pop an element
# Output: random element
print(my_set.pop())

# pop another element
my_set.pop()
print(my_set)

# clear my_set
# Output: set()
my_set.clear()
print(my_set)

print(my_set)
```

**Output**
```
{'H', 'l', 'r', 'W', 'o', 'd', 'e'}
H
{'r', 'W', 'o', 'd', 'e'}
set()
```
#### Set Operations

##### Union


```python
# Intersection of sets
# initialize A and B
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

# use & operator
# Output: {4, 5}
print(A & B)

# use intersection function on A
>>> A.intersection(B)
{4, 5}

# use intersection function on B
>>> B.intersection(A)
{4, 5}
```

##### Difference


```python
# Difference of two sets
# initialize A and B
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

# use - operator on A
# Output: {1, 2, 3}
print(A - B)

# use difference function on A
>>> A.difference(B)
{1, 2, 3}

# use - operator on B
>>> B - A
{8, 6, 7}

# use difference function on B
>>> B.difference(A)
{8, 6, 7}
```

##### Symmetric Difference


Symmetric Difference of A and B is a set of elements in A and B but not in both (excluding the intersection).

Symmetric difference is performed using `^` operator. Same can be accomplished using the method `symmetric_difference()`.

```python
# Symmetric difference of two sets
# initialize A and B
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

# use ^ operator
# Output: {1, 2, 3, 6, 7, 8}
print(A ^ B)

# use symmetric_difference function on A
>>> A.symmetric_difference(B)
{1, 2, 3, 6, 7, 8}

# use symmetric_difference function on B
>>> B.symmetric_difference(A)
{1, 2, 3, 6, 7, 8}
```

#### Other Set Methods

| Method                                                       | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [add()](https://www.programiz.com/python-programming/methods/set/add) | Adds an element to the set                                   |
| [clear()](https://www.programiz.com/python-programming/methods/set/clear) | Removes all elements from the set                            |
| [copy()](https://www.programiz.com/python-programming/methods/set/copy) | Returns a copy of the set                                    |
| [difference()](https://www.programiz.com/python-programming/methods/set/difference) | Returns the difference of two or more sets as a new set      |
| [difference_update()](https://www.programiz.com/python-programming/methods/set/difference_update) | Removes all elements of another set from this set            |
| [discard()](https://www.programiz.com/python-programming/methods/set/discard) | Removes an element from the set if it is a member. (Do nothing if the element is not in set) |
| [intersection()](https://www.programiz.com/python-programming/methods/set/intersection) | Returns the intersection of two sets as a new set            |
| [intersection_update()](https://www.programiz.com/python-programming/methods/set/intersection_update) | Updates the set with the intersection of itself and another  |
| [isdisjoint()](https://www.programiz.com/python-programming/methods/set/isdisjoint) | Returns `True` if two sets have a null intersection          |
| [issubset()](https://www.programiz.com/python-programming/methods/set/issubset) | Returns `True` if another set contains this set              |
| [issuperset()](https://www.programiz.com/python-programming/methods/set/issuperset) | Returns `True` if this set contains another set              |
| [pop()](https://www.programiz.com/python-programming/methods/set/pop) | Removes and returns an arbitrary set element. Raises `KeyError` if the set is empty |
| [remove()](https://www.programiz.com/python-programming/methods/set/remove) | Removes an element from the set. If the element is not a member, raises a `KeyError` |
| [symmetric_difference()](https://www.programiz.com/python-programming/methods/set/symmetric_difference) | Returns the symmetric difference of two sets as a new set    |
| [symmetric_difference_update()](https://www.programiz.com/python-programming/methods/set/symmetric_difference_update) | Updates a set with the symmetric difference of itself and another |
| [union()](https://www.programiz.com/python-programming/methods/set/union) | Returns the union of sets in a new set                       |
| [update()](https://www.programiz.com/python-programming/methods/set/update) | Updates the set with the union of itself and others          |

##### Set Membership Test
```python
# in keyword in a set
# initialize my_set
my_set = set("apple")

# check if 'a' is present
# Output: True
print('a' in my_set)

# check if 'p' is present
# Output: False
print('p' not in my_set)
```

##### Iterating Through a Set

```python
>>> for letter in set("apple"):
...     print(letter)
...    
a
p
e
l
```

##### Built-in Functions with Set
Built-in functions like `all()`, `any()`, `enumerate()`, `len()`, `max()`, `min()`, `sorted()`, `sum()` etc. are commonly used with sets to perform different tasks.

| Function                                                     | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [all()](https://www.programiz.com/python-programming/methods/built-in/all) | Returns `True` if all elements of the set are true (or if the set is empty). |
| [any()](https://www.programiz.com/python-programming/methods/built-in/any) | Returns `True` if any element of the set is true. If the set is empty, returns `False`. |
| [enumerate()](https://www.programiz.com/python-programming/methods/built-in/enumerate) | Returns an enumerate object. It contains the index and value for all the items of the set as a pair. |
| [len()](https://www.programiz.com/python-programming/methods/built-in/len) | Returns the length (the number of items) in the set.         |
| [max()](https://www.programiz.com/python-programming/methods/built-in/max) | Returns the largest item in the set.                         |
| [min()](https://www.programiz.com/python-programming/methods/built-in/min) | Returns the smallest item in the set.                        |
| [sorted()](https://www.programiz.com/python-programming/methods/built-in/sorted) | Returns a new sorted list from elements in the set(does not sort the set itself). |
| [sum()](https://www.programiz.com/python-programming/methods/built-in/sum) | Returns the sum of all elements in the set.                  |

##### Frozenset

Frozenset is a new class that has the characteristics of a set, but its elements cannot be changed once assigned. While tuples are immutable lists, frozensets are immutable sets.

Sets being mutable are unhashable, so they can't be used as dictionary keys. On the other hand, frozensets are hashable and can be used as keys to a dictionary.

Frozensets can be created using the [frozenset()](https://www.programiz.com/python-programming/methods/built-in/frozenset) function.

This data type supports methods like `copy()`, `difference()`, `intersection()`, `isdisjoint()`, `issubset()`, `issuperset()`, `symmetric_difference()` and `union()`. Being immutable, it does not have methods that add or remove elements.

```python
# Frozensets
# initialize A and B
A = frozenset([1, 2, 3, 4])
B = frozenset([3, 4, 5, 6])

>>> A.isdisjoint(B)
False
>>> A.difference(B)
frozenset({1, 2})
>>> A | B
frozenset({1, 2, 3, 4, 5, 6})
>>> A.add(3)
...
AttributeError: 'frozenset' object has no attribute 'add'
```

### Dictionary

Creating a dictionary is as simple as placing items inside curly braces {} separated by commas.

Python dictionary is an unordered collection of items. Each item of a dictionary has a `key/value` pair.

Dictionaries are optimized to retrieve values when the key is known.

```python
# empty dictionary
my_dict = {}

# dictionary with integer keys
my_dict = {1: 'apple', 2: 'ball'}

# dictionary with mixed keys
my_dict = {'name': 'John', 1: [2, 4, 3]}

# using dict()
my_dict = dict({1:'apple', 2:'ball'})

# from sequence having each item as a pair
my_dict = dict([(1,'apple'), (2,'ball')])

# get vs [] for retrieving elements
my_dict = {'name': 'Jack', 'age': 26}

# Output: Jack
print(my_dict['name'])

# Output: 26
print(my_dict.get('age'))

# Trying to access keys which doesn't exist throws error
# Output None
print(my_dict.get('address'))

# KeyError
print(my_dict['address'])
```

##### Adding elements

```python
# Changing and adding Dictionary Elements
my_dict = {'name': 'Jack', 'age': 26}

# update value
my_dict['age'] = 27

#Output: {'age': 27, 'name': 'Jack'}
print(my_dict)

# add item
my_dict['address'] = 'Downtown'

# Output: {'address': 'Downtown', 'age': 27, 'name': 'Jack'}
print(my_dict)
```

##### Removing elements from Dictionary

We can remove a particular item in a dictionary by using the `pop()` method. This method removes an item with the provided `key` and returns the `value`.

The `popitem()` method can be used to remove and return an arbitrary `(key, value)` item pair from the dictionary. All the items can be removed at once, using the `clear()` method.

We can also use the `del` keyword to remove individual items or the entire dictionary itself.

```python
# Removing elements from a dictionary

# create a dictionary
squares = {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}

# remove a particular item, returns its value
# Output: 16
print(squares.pop(4))

# Output: {1: 1, 2: 4, 3: 9, 5: 25}
print(squares)

# remove an arbitrary item, return (key,value)
# Output: (5, 25)
print(squares.popitem())

# Output: {1: 1, 2: 4, 3: 9}
print(squares)

# remove all items
squares.clear()

# Output: {}
print(squares)

# delete the dictionary itself
del squares

# Throws Error
print(squares)
```

**Output**
```
16
{1: 1, 2: 4, 3: 9, 5: 25}
(5, 25)
{1: 1, 2: 4, 3: 9}
{}
Traceback (most recent call last):
  File "<string>", line 30, in <module>
    print(squares)
NameError: name 'squares' is not defined
```

##### Dictionary Methods

| Method                                                       | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [clear()](https://www.programiz.com/python-programming/methods/dictionary/clear) | Removes all items from the dictionary.                       |
| [copy()](https://www.programiz.com/python-programming/methods/dictionary/copy) | Returns a shallow copy of the dictionary.                    |
| Fromkeys(seq[,v])                                            | Returns a new dictionary with `keys` from `seq` and value equal to `v` (defaults to `None`). |
| get(key[,d])                                                 | Returns the value of the `key`. If the `key` does not exist, returns `d` (defaults to `None`). |
| [items()](https://www.programiz.com/python-programming/methods/dictionary/items) | Return a new object of the dictionary's items in (key, value) format. |
| [keys()](https://www.programiz.com/python-programming/methods/dictionary/keys) | Returns a new object of the dictionary's keys.               |
| [pop(key[,d\])](https://www.programiz.com/python-programming/methods/dictionary/pop) | Removes the item with the `key` and returns its value or `d` if `key` is not found. If `d` is not provided and the `key` is not found, it raises `KeyError`. |
| [popitem()](https://www.programiz.com/python-programming/methods/dictionary/popitem) | Removes and returns an arbitrary item (**key, value**). Raises `KeyError` if the dictionary is empty. |
| setdefault(key[,d\])](https://www.programiz.com/python-programming/methods/dictionary/setdefault) | Returns the corresponding value if the key is in the dictionary. If not, inserts the key with a value of d and returns d (defaults to `None`). |
| [update([other\])](https://www.programiz.com/python-programming/methods/dictionary/update) | Updates the dictionary with the key/value pairs from other, overwriting existing keys. |
| [values()](https://www.programiz.com/python-programming/methods/dictionary/values) | Returns a new object of the dictionary's values              |

| Function                                                     | Description                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [all()](https://www.programiz.com/python-programming/methods/built-in/all) | Return `True` if all keys of the dictionary are True (or if the dictionary is empty). |
| [any()](https://www.programiz.com/python-programming/methods/built-in/any) | Return `True` if any key of the dictionary is true. If the dictionary is empty, return `False`. |
| [len()](https://www.programiz.com/python-programming/methods/built-in/len) | Return the length (the number of items) in the dictionary.   |
| cmp()                                                        | Compares items of two dictionaries. (Not available in Python 3) |
| [sorted()](https://www.programiz.com/python-programming/methods/built-in/sorted) | Return a new sorted list of keys in the dictionary.          |



##### Dictionary Comprehension
Dictionary comprehension is an elegant and concise way to create a new dictionary from an iterable in Python.

Dictionary comprehension consists of an expression pair `(key: value)` followed by a `for` statement inside curly braces `{}`.

```python
# Dictionary Comprehension
squares = {x: x*x for x in range(6)}

print(squares)
```
**Output**
```
{0: 0, 1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```
This code is equivalent to
```python
squares = {}
for x in range(6):
    squares[x] = x*x
print(squares)
```
**Output**
```
{0: 0, 1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```


## Input, Output and Import
Python provides numerous [built-in functions](https://www.programiz.com/python-programming/methods/built-in) that are readily available to us at the Python prompt.

Some of the functions like `input()` and `print()` are widely used for standard input and output operations respectively.

### Output
##### Output Using print() function
We use the `print()` function to output data to the standard output device (screen). We can also [output data to a file](https://www.programiz.com/python-programming/file-operation).
```python

print('This sentence is output to the screen')
```
***Output***
```
This sentence is output to the screen
```
Another example is given below:
```python
a = 5
print('The value of a is', a)
```
***Output***
```
The value of a is 5
```
##### Output formatting
Sometimes we would like to format our output to make it look attractive. This can be done by using the `str.format()` method. This method is visible to any string object.
```python
>>> x = 5; y = 10
>>> print('The value of x is {} and y is {}'.format(x,y))
The value of x is 5 and y is 10

print('I love {0} and {1}'.format('bread','butter'))
print('I love {1} and {0}'.format('bread','butter'))
```
Here, the curly braces `{}` are used as placeholders. We can specify the order in which they are printed by using numbers (tuple index).
**Output**
```
I love bread and butter
I love butter and bread
```

### Input
Up until now, our programs were static. The value of variables was defined or hard coded into the source code.

To allow flexibility, we might want to take the input from the user. In Python, we have the `input()` function to allow this. The syntax for `input()` is:
```python
>>> num = input('Enter a number: ')
Enter a number: 10
>>> num
'10'


>>> int('10')
10
>>> float('10')
10.0

>>> int('2+3')
Traceback (most recent call last):
  File "<string>", line 301, in runcode
  File "<interactive input>", line 1, in <module>
ValueError: invalid literal for int() with base 10: '2+3'
>>> eval('2+3')
5
```

###  Import
When our program grows bigger, it is a good idea to break it into different modules.

A module is a file containing Python definitions and statements. [Python modules](https://www.programiz.com/python-programming/modules) have a filename and end with the extension `.py`.

Definitions inside a module can be imported to another module or the interactive interpreter in Python. We use the `import` keyword to do this.

```python
import math
print(math.pi)
#Output
3.141592653589793

>>> from math import pi
>>> pi
3.141592653589793
```


## Operators

### Arithmetic operators

Arithmetic operators are used to perform mathematical operations like addition, subtraction, multiplication, etc.

| Operator | Meaning                                                      | Example                  |
| :------- | :----------------------------------------------------------- | :----------------------- |
| +        | Add two operands or unary plus                               | x + y+ 2                 |
| -        | Subtract right operand from the left or unary minus          | x - y- 2                 |
| *        | Multiply two operands                                        | x * y                    |
| /        | Divide left operand by the right one (always results into float) | x / y                    |
| %        | Modulus - remainder of the division of left operand by the right | x % y (remainder of x/y) |
| //       | Floor division - division that results into whole number adjusted to the left in the number line | x // y                   |
| **       | Exponent - left operand raised to the power of right         | x**y (x to the power y)  |

### Comparison operators

Comparison operators are used to compare values. It returns either `True` or `False` according to the condition.

| Operator | Meaning                                                      | Example |
| :------- | :----------------------------------------------------------- | :------ |
| >        | Greater than - True if left operand is greater than the right | x > y   |
| <        | Less than - True if left operand is less than the right      | x < y   |
| ==       | Equal to - True if both operands are equal                   | x == y  |
| !=       | Not equal to - True if operands are not equal                | x != y  |
| >=       | Greater than or equal to - True if left operand is greater than or equal to the right | x >= y  |
| <=       | Less than or equal to - True if left operand is less than or equal to the right | x <= y  |

**Example**
```python
x = 10
y = 12

# Output: x > y is False
print('x > y is',x>y)

# Output: x < y is True
print('x < y is',x<y)

# Output: x == y is False
print('x == y is',x==y)

# Output: x != y is True
print('x != y is',x!=y)

# Output: x >= y is False
print('x >= y is',x>=y)

# Output: x <= y is True
print('x <= y is',x<=y)
```
**Output**
```
x > y is False
x < y is True
x == y is False
x != y is True
x >= y is False
x <= y is True
```

### Logical operators
Logical operators are the `and`, `or`, `not` operators.

| Operator | Meaning                                            | Example |
| :------- | :------------------------------------------------- | :------ |
| and      | True if both the operands are true                 | x and y |
| or       | True if either of the operands is true             | x or y  |
| not      | True if operand is false (complements the operand) | not x   |

```python

x = True
y = False

print('x and y is',x and y)

print('x or y is',x or y)

print('not x is',not x)
```
**Output**
```
x and y is False
x or y is True
not x is False
```
### Bitwise operators

Bitwise operators act on operands as if they were strings of binary digits. They operate bit by bit, hence the name.

For example, `2` is `10` in binary and `7` is `111`.

**In the table below:** Let x = 10 (`0000 1010` in binary) and y = 4 (`0000 0100` in binary)

| Operator | Meaning             | Example                   |
| :------- | :------------------ | :------------------------ |
| &        | Bitwise AND         | x & y = 0 (`0000 0000`)   |
| \|       | Bitwise OR          | x \| y = 14 (`0000 1110`) |
| ~        | Bitwise NOT         | ~x = -11 (`1111 0101`)    |
| ^        | Bitwise XOR         | x ^ y = 14 (`0000 1110`)  |
| >>       | Bitwise right shift | x >> 2 = 2 (`0000 0010`)  |
| <<       | Bitwise left shift  | x << 2 = 40 (`0010 1000`) |

------
### Assignment operators

Assignment operators are used in Python to assign values to variables.

`a = 5` is a simple assignment operator that assigns the value 5 on the right to the variable `a` on the left.

There are various compound operators in Python like `a += 5` that adds to the variable and later assigns the same. It is equivalent to `a = a + 5`.


| Operator | Example | Equivalent to |
| :------- | :------ | :------------ |
| =        | x = 5   | x = 5         |
| +=       | x += 5  | x = x + 5     |
| -=       | x -= 5  | x = x - 5     |
| *=       | x *= 5  | x = x * 5     |
| /=       | x /= 5  | x = x / 5     |
| %=       | x %= 5  | x = x % 5     |
| //=      | x //= 5 | x = x // 5    |
| **=      | x **= 5 | x = x ** 5    |
| &=       | x &= 5  | x = x & 5     |
| \|=      | x \|= 5 | x = x \| 5    |
| ^=       | x ^= 5  | x = x ^ 5     |
| >>=      | x >>= 5 | x = x >> 5    |
| <<=      | x <<= 5 | x = x << 5    |
------

### Special operators

Python language offers some special types of operators like the identity operator or the membership operator. They are described below with examples.

#### Identity operators

`is` and `is not` are the identity operators in Python. They are used to check if two values (or variables) are located on the same part of the memory. Two variables that are equal does not imply that they are identical.

| Operator | Meaning                                                      | Example       |
| :------- | :----------------------------------------------------------- | :------------ |
| is       | True if the operands are identical (refer to the same object) | x is True     |
| is not   | True if the operands are not identical (do not refer to the same object) | x is not True |

**Example**

```python
x1 = 5
y1 = 5
x2 = 'Hello'
y2 = 'Hello'
x3 = [1,2,3]
y3 = [1,2,3]

# Output: False
print(x1 is not y1)

# Output: True
print(x2 is y2)

# Output: False
print(x3 is y3)
```
**Output**
```
False
True
False
```

Here, we see that `x1` and `y1` are integers of the same values, so they are equal as well as identical. Same is the case with `x2` and `y2` (strings).

But `x3` and `y3` are lists. They are equal but not identical. It is because the interpreter locates them separately in memory although they are equal.

-----

#### Membership operators

`in` and `not in` are the membership operators in Python. They are used to test whether a value or variable is found in a sequence ([string](https://www.programiz.com/python-programming/string), [list](https://www.programiz.com/python-programming/list), [tuple](https://www.programiz.com/python-programming/tuple), [set](https://www.programiz.com/python-programming/set) and [dictionary](https://www.programiz.com/python-programming/dictionary)).

In a dictionary we can only test for presence of key, not the value.
| Operator | Meaning                                             | Example    |
| :------- | :-------------------------------------------------- | :--------- |
| in       | True if value/variable is found in the sequence     | 5 in x     |
| not in   | True if value/variable is not found in the sequence | 5 not in x |

**Example**
```python
x = 'Hello world'
y = {1:'a',2:'b'}

# Output: True
print('H' in x)

# Output: True
print('hello' not in x)

# Output: True
print(1 in y)

# Output: False
print('a' in y)
```
**Output**
```
True
True
True
False
```

Here, `'H'` is in `x` but `'hello'` is not present in `x` (remember, Python is case sensitive). Similarly, `1` is key and `'a'` is the value in dictionary `y`. Hence, `'a' in y` returns `False`.

# Control flow

## if...else Statement
```python 
if expression:
  statement(s)
elif expression:
  statement(s)
elif expression:
  statement(s)
else:
  statement(s)
```

## for Loop
```python
for val in sequence:
    loop body
```

### The range() function

We can generate a sequence of numbers using `range()` function. `range(10)` will generate numbers from 0 to 9 (10 numbers).

We can also define the start, stop and step size as `range(start, stop,step_size)`. step_size defaults to 1 if not provided.

The `range` object is "lazy" in a sense because it doesn't generate every number that it "contains" when we create it. However, it is not an iterator since it supports `in`, `len` and `__getitem__` operations.

This function does not store all the values in memory; it would be inefficient. So it remembers the start, stop, step size and generates the next number on the go.

To force this function to output all the items, we can use the function `list()`.

The following example will clarify this.
```python
print(range(10))

print(list(range(10)))

print(list(range(2, 8)))

print(list(range(2, 20, 3)))
```

**Output**
```
range(0, 10)
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
[2, 3, 4, 5, 6, 7]
[2, 5, 8, 11, 14, 17]
```

#### for loop with else

```python
digits = [0, 1, 5]

for i in digits:
    print(i)
else:
    print("No items left.")
```

## while Loop
```python
while expression:
	Body of while
  

while expression:
  Body of while
else:
  # while loop's else part runs if no break occurs and the condition is false.
```

## break statement

The `break` statement terminates the loop containing it. Control of the program flows to the statement immediately after the body of the loop.

If the `break` statement is inside a nested loop (loop inside another loop), the break statement will terminate the innermost loop.

### Syntax of break
```
break
```

### Flowchart of break

![Flowchart of break statement in Python](https://cdn.programiz.com/sites/tutorial2program/files/flowchart-break-statement.jpg)

The working of break statement in [for loop](https://www.programiz.com/python-programming/for-loop) and [while loop](https://www.programiz.com/python-programming/while-loop) is shown below.

![How the break statement works in Python](https://cdn.programiz.com/sites/tutorial2program/files/how-break-statement-works.jpg)

**Example**
```python
# Use of break statement inside the loop

for val in "string":
    if val == "i":
        break
    print(val)

print("The end")
```

**Output**
```
s
t
r
The end
```

## continue statement
The `continue` statement is used to skip the rest of the code inside a loop for the current iteration only. Loop does not terminate but continues on with the next iteration.

### Syntax of Continue
```
continue
```

### Flowchart of continue 
![Flowchart of continue statement in Python](https://cdn.programiz.com/sites/tutorial2program/files/continue-statement-flowchart.jpg)

The working of continue statement in for and while loop is shown below.

![How continue statement works in python](https://cdn.programiz.com/sites/tutorial2program/files/how-continue-statment-works.jpg)

**Example**
```python
# Program to show the use of continue statement inside loops

for val in "string":
    if val == "i":
        continue
    print(val)

print("The end")
```

**Output**
```
s
t
r
n
g
The end
```
This program is same as the above example except the `break` statement has been replaced with `continue`.

We continue with the loop, if the string is `i`, not executing the rest of the block. Hence, we see in our output that all the letters except `i` gets printed.

## What is pass statement in Python?

In Python programming, the `pass` statement is a null statement. The difference between a [comment](https://www.programiz.com/python-programming/statement-indentation-comments) and a `pass` statement in Python is that while the interpreter ignores a comment entirely, `pass` is not ignored.

However, nothing happens when the pass is executed. It results in no operation (NOP).

### Syntax of pass
```
pass
```

**Example**
```python
class Animals:
  pass

for item in list:
  pass

def eat():
  pass
```

# Functions

In Python, a function is a group of related statements that performs a specific task.

Functions help break our program into smaller and modular chunks. As our program grows larger and larger, functions make it more organized and manageable.

Furthermore, it avoids repetition and makes the code reusable.

**Syntax**
```python
def function_name(parameters):
	"""docstring"""
	statement(s)

# Function with return value
def functionName(parameters):
  statement(s)
  return parameters
```
### Python Arbitrary Arguments

Sometimes, we do not know in advance the number of arguments that will be passed into a function. Python allows us to handle this kind of situation through function calls with an arbitrary number of arguments.

In the function definition, we use an asterisk (*) before the parameter name to denote this kind of argument. Here is an example.
```
def greet(*names):
    """This function greets all
    the person in the names tuple."""

    # names is a tuple with arguments
    for name in names:
        print("Hello", name)


greet("Monica", "Luke", "Steve", "John")
```

**Output**
```
Hello Monica
Hello Luke
Hello Steve
Hello John
```

Here, we have called the function with multiple arguments. These arguments get wrapped up into a tuple before being passed into the function. Inside the function, we use a `for` loop to retrieve all the arguments back.

## Recursion

Recursion is the process of defining something in terms of itself.

A physical world example would be to place two parallel mirrors facing each other.Any object in between them would be reflected recursively.

Factorial of a number is the product of all the integers from 1 to that number. For example, the factorial of 6 (denoted as 6!) is 1*2*3*4*5*6 = 720.

**Example**
```python
def factorial(x):
    """This is a recursive function
    to find the factorial of an integer"""

    if x == 1:
        return 1
    else:
        return (x * factorial(x-1))


num = 3
print("The factorial of", num, "is", factorial(num))
```
**Output**
```
The factorial of 3 is 6
```

When we call this function with a positive integer, it will recursively call itself by decreasing the number.

Each function multiplies the number with the factorial of the number below it until it is equal to one. This recursive call can be explained in the following steps.

```
factorial(3)          # 1st call with 3
3 * factorial(2)      # 2nd call with 2
3 * 2 * factorial(1)  # 3rd call with 1
3 * 2 * 1             # return from 3rd call as number=1
3 * 2                 # return from 2nd call
6                     # return from 1st call
```

### Advantages of Recursion

1. Recursive functions make the code look clean and elegant.
2. A complex task can be broken down into simpler sub-problems using recursion.
3. Sequence generation is easier with recursion than using some nested iteration.

-----

### Disadvantages of Recursion
1. Sometimes the logic behind recursion is hard to follow through.
2. Recursive calls are expensive (inefficient) as they take up a lot of memory and time.
3. Recursive functions are hard to debug.

##  Anonymous/Lambda Function

In Python, an anonymous function is a [function](https://www.programiz.com/python-programming/function) that is defined without a name.

While normal functions are defined using the `def` keyword in Python, anonymous functions are defined using the `lambda` keyword.

Hence, anonymous functions are also called lambda functions.

**Syntax**
```
lambda arguments: expression
```
Lambda functions can have any number of arguments but only one expression. The expression is evaluated and returned. Lambda functions can be used wherever function objects are required.

**Example**
```python
# Program to show the use of lambda functions
double = lambda x: x * 2

# Output: 10
print(double(5))
```

In the above program, `lambda x: x * 2` is the lambda function. Here `x` is the argument and `x * 2` is the expression that gets evaluated and returned.

This function has no name. It returns a function object which is assigned to the identifier `double`. We can now call it as a normal function. The statement

```
double = lambda x: x * 2
```
is nearly the same as:
```
def double(x):
   return x * 2
```

### Use of Lambda Function in python

We use lambda functions when we require a nameless function for a short period of time.

In Python, we generally use it as an argument to a higher-order function (a function that takes in other functions as [arguments](https://www.programiz.com/python-programming/function-argument)). Lambda functions are used along with built-in functions like `filter()`, `map()` etc.

### Example use with filter()

The `filter()` function in Python takes in a function and a list as arguments.

The function is called with all the items in the list and a new list is returned which contains items for which the function evaluates to `True`.

Here is an example use of `filter()` function to filter out only even numbers from a list.







