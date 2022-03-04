# The Reeves programming language

***

The Reeves programming language is a easy to compiled language
language that can be compiled to python code

## Getting started

### Unix

First things first, you need to install the reeves
compiler. You can do a git clone to copy the repo

```bash
git clone https://github.com/someStranger8/Reeves
cd Reeves
```

and then you can add it to you binarys folder

```
# check for naming issues
ls /bin | grep reeves

# add it to your binarys folder
sudo cp reeves /bin
```

### Windows

To download the reeves compiler from
the github page. Next navigate to the file
and add it to your system32

```
copy C:\PATH\TO\FILE\reeves D:\Windows\System32
```

## Syntax

***

you can compile a file to python

```bash
$ reeves MyFile.ree
```

you can join strings together

```python
var my_var = "name"
print("hello" + name)
```

you can use indentation of 2 or 4 spaces

```python
if x < 5:
  print("x is less than five")
```

or you can also use the `end` key word
to end a if statment, function, etc...

```python
if x < 5 then
  print("x is less than 5")
end

# this works too
if x < 5 then print("x is less than 5") end
```

## Comments

***

Comments are very simple you can use a `#`,
example:

```python
# this is a comment

print("hi") # this works
```

you can also use multi line comments:

```python
"""
this is a multi line
comment
"""
```

## Varibles

***

reeves has varibles which you can assign to a value

```python
my_var = 1
```

you can also use the `var` keyword

```python
var my_var = 1
```

you can assign specific data types to varibles

```python
var a = int(6)
var b = str("hello")
var c = float(3.14159)
```

## Functions

***

to define a function you use the `func` key word

```python
func myFunc():
  print("hi")

# this works too
func myFunc() then
  print("hi")
end
```

you can also pass parameters

```python
func add(a, b):
   print(a + b)
```

you can also use the `return` keyword

```python
func add(a, b):
  return a + b
```

you can call functions like this:

```python
func add(a, b):
  return a + b

print(add(1, 1))

# or just normaly like this:
add(1, 1)
```

## Booleans

***

booleans are realy simple

```python
# this works
var hi = True

# and this
var hello = true

# you can do this
if hello == False:
  print("hello")

# or
while false:
  print("lol")
```

## If...else

***

you can use if else statments like this

```python
n = 0

if n == 1:
  print("hi")

else:
  print(":(")
```

you can also use `elif`

```python
n = 0

if n == 0:
  print("hi")

elif n == 1:
  print("nice")

else:
  print(":(")
```

you can also use other logical expressions other than `==`

```python
# like this
if n < 5 then
  # do something
end
```

## While

***

the `while` key word is very simple
you have the `while` keyword and then a logical expresion
while the logical expresion is true it executes that code

```python
while True:
  print("hello")

# this works too
while True then
  # do something
end
```

## For

***

You can use the `for` keyword like this:

```python
for i in myVarible:
  # do something

# this also works
for i in myVarible then
  # do something
end
```

you can also use the `range()` function

```python
for i in range(100):
  # does this 100 times
```

## Classes

***

In reeves you can use classes for OOP

```python
# initalize the dog class
class Dog():
  func init(self, name):
    self.name = name

  func bark(self):
    print("bark bark bark")
```

to call a class you can use

```python
var myDog = new Dog("henry")
myDog.bark()
```

## Modules

***

say i have a file called `myFile.ree`
> NOTE: to import a module you have to compile it to python code

i can import it using the `import` keyword

`myFile.ree` :

```python
func hello():
  print("hello")
```

i can do:

```python
import myFile
myFile.hello()
```

you can import a specific function or all of them

```python
from myFile import hello

# or you can import all the functions

from myFile import *
```

classes work too

```python
from myFile import *
var dog = new Dog("henry")
dog.bark()
```

## Math

***

> `+` : addition<br>

`-` : subtraction<br>

`*`: multiplication<br>

`/` : division<br>

`^` : exponents

you can also import the built in<br>

math module for other stuff

## String formating

***

you can format strings bt doing

```python
var price = 42
txt = "the price of a apple is {} cents"
print(txt.format(price)
```

or

```python
var price = 42
txt = f"the price is {price}"
print(txt)
```

## I/O

***

you can use the `print()` function to print something<br>

to the console like `console.log()` here is<br>

an example:

```python
print("hi")
```

you can also print out varible

```python
var hi = "hi"
print(hi)
```

you can also get user input

```python
input("whats you name? ")
```

you can save that user input<br>

as a varible

```python
user_input = input("hello")
print(user_input)
```

you can also access the file system using the open function

```python
var f = open("hello.gdoc", "r")
```

## List and dictonaries

***

you can create a list in reeves like<br>

this:

```python
myList = [1,2,3,4,5,6]
```

and you can make dictonarys like this:

```python
myDict = {
    "key":"value",
    "thing1":"thing2"
}
```

## Try...except

try and except in reeves is realy simple

```python
try:
  import module as mod
  mod.func()

# you can also do this
except ImportError then
  print("sorry there was an error")
end
```

***

## Logical expressions

***

> Equals: `a == b`<br>

Not Equals: `a != b`<br>

Less than: `a < b`<br>

Less than or equal to: `a =< b`<br>

Greater than: `a > b`<br>

Greater than or equal to: `a >= b`<br>

`and`<br>

`is`<br>

`or`<br>

`in`

## Data types

***

varibles have different data types:

> Text types: `str`<br>

Numeric types: `int`, `float`, `complex`<br>

Sequence types: `list`, `range`<br>

Mapping types: `dict`<br>

Set types: `set`, `frozenset`<br>

Boolean type: `bool`<br>

Binary types: `byte`, `bytearray`, `memoryview`
