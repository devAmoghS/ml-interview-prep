### 1) What is Python? What are the benefits of using Python?

Python is a programming language with objects, modules, threads, exceptions and automatic memory management. The benefits of pythons are that it is simple and easy
, portable
, extensible
, build-in data structure 
and it is an open source.

### 2) What is ```PEP 8```?

```PEP 8``` is a coding convention, a set of recommendation, about how to write your Python code more readable.

### 3) What is pickling and unpickling?

```Pickle``` module accepts any Python object and converts it into a string representation and dumps it into a file by using dump function, this process is called ```pickling```. While the process of retrieving original Python objects from the stored string representation is called ```unpickling```.

### 4) How Python is interpreted?

Python language is an interpreted language. Python program runs directly from the source code. It converts the source code that is written by the programmer into an intermediate language, which is again translated into machine language that has to be executed.

### 5) How memory is managed in Python?

Python memory is managed by **Python private heap space**. All Python objects and data structures are located in a private heap. The programmer **does not have an access** to this private heap and **interpreter takes care** of this Python private heap.
The allocation of Python heap space for Python objects is done by **Python memory manager**. The core API gives access to some tools for the programmer to code.
Python also have an **inbuilt garbage collector**, which recycle all the unused memory and frees the memory and makes it available to the heap space.

### 6) What are the tools that help to find bugs or perform static analysis?

PyChecker is a static analysis tool that detects the bugs in Python source code and warns about the style and complexity of the bug. Pylint is another tool that verifies whether the module meets the coding standard.

### 7) What are Python decorators?

A Python decorator is a specific change that we make in Python syntax to alter functions easily.

### 8) What is the difference between list and tuple?

The difference between list and tuple is that list is mutable while tuple is not. Tuple can be hashed for e.g as a key for dictionaries.

### 9) How are arguments passed by value or by reference?

Everything in Python is an object and all variables hold references to the objects. The references values are according to the functions; as a result you cannot change the value of the references. However, you can change the objects if it is mutable.

### 10) What is Dict and List comprehensions are?

They are syntax constructions to ease the creation of a Dictionary or List based on existing iterable.

### 11) What are the built-in type does python provides?
There are mutable and Immutable types of Pythons built in types 

#### Mutable built-in types

* List
* Sets
* Dictionaries

#### Immutable built-in types

* Strings
* Tuples
* Numbers

### 12) What is namespace in Python?

In Python, every name introduced has a place where it lives and can be hooked for. This is known as namespace. It is like a box where a variable name is mapped to the object placed. Whenever the variable is searched out, this box will be searched, to get corresponding object.

### 13) What is lambda in Python?

It is a single expression anonymous function often used as inline function.

### 14) Why lambda forms in python does not have statements?

A lambda form in python does not have statements as it is used to make new function object and then return them at runtime.

### 15) What is ```pass``` in Python?

Pass means, no-operation Python statement, or in other words it is a place holder in compound statement, where there should be a blank left and nothing has to be written there.

### 16) In Python what are iterators?

In Python, iterators are used to iterate a group of elements, containers like list.

### 17) What is unittest in Python?

A unit testing framework in Python is known as ```unittest```. It supports sharing of setups, automation testing, shutdown code for tests, aggregation of tests into collections etc.

### 18) In Python what is slicing?

A mechanism to select a range of items from sequence types like list, tuple, strings etc. is known as slicing.

### 19) What are generators in Python?

The way of implementing iterators are known as generators. It is a normal function except that it yields expression in the function.

__From RealPython__:
generator functions are a special kind of function that return a lazy iterator. These are objects that you can loop over like a list. However, unlike lists, lazy iterators do not store their contents in memory.

Generator functions use the Python ```yield``` keyword instead of ```return```

```
def infinite_sequence():
    num = 0
    while True:
        yield num
        num += 1
```

```yield``` indicates where a value is sent back to the caller, but unlike ```return```, you don’t exit the function afterward.

Instead, the **state** of the function is remembered. That way, when ```next()``` is called on a generator object (either explicitly or implicitly within a for loop), the previously yielded variable ```num``` is incremented, and then yielded again

More at: https://realpython.com/introduction-to-python-generators/

### 20) What is docstring in Python?
### 21) How can you copy an object in Python?

To copy an object in Python, you can try ```copy.copy ()``` or ```copy.deepcopy()``` for the general case. You cannot copy all objects but most of them.

* A **shallow copy** means constructing a new collection object and then populating it with references to the child objects found in the original. In essence, a shallow copy is only one level deep. The copying process does not recurse and therefore won’t create copies of the child objects themselves.

* A **deep copy** makes the copying process recursive. It means first constructing a new collection object and then recursively populating it with copies of the child objects found in the original. Copying an object this way walks the whole object tree to create a fully independent clone of the original object and all of its children.

### 22) What is negative index in Python?

Python sequences can be index in positive and negative numbers. For positive index, 0 is the first index, 1 is the second index and so forth. For negative index, (-1) is the last index and (-2) is the second last index and so forth.

### 23) How you can convert a number to a string?

In order to convert a number into a string, use the inbuilt function ```str()```. If you want a octal or hexadecimal representation, use the inbuilt function ```oct()``` or ```hex()```.

### 24) What is the difference between Xrange and range?

```Xrange``` returns the xrange object while ```range``` returns the list, and uses the same memory and no matter what the range size is.

__From Stack Overflow__ : It is for optimization reasons.

```range()``` will create a list of values from start to end (0 .. 20 in your example). This will become an expensive operation on very large ranges.

```xrange()``` on the other hand is much more optimised. it will only compute the next value when needed (via an xrange sequence object) and does not create a list of all values like range() does

### 25) What is module and package in Python?

In Python, module is the way to structure program. Each Python program file is a module, which imports other modules like objects and attributes.

The folder of Python program is a package of modules. A package can have modules or subfolders.

### 26) Mention what are the rules for local and global variables in Python?

**Local variables**: If a variable is assigned a new value anywhere within the function's body, it's assumed to be local.

**Global variables**: Those variables that are only referenced inside a function are implicitly global.

### 27) How can you share global variables across modules?

To share global variables across modules within a single program, create a special module. Import the config module in all modules of your application. The module will be available as a global variable across modules.

### 28) Explain how can you make a Python Script executable on Unix?
### 29) Explain how to delete a file in Python?

By using a command ```os.remove (filename)``` or ```os.unlink(filename)```

### 30) Explain how can you generate random numbers in Python?

To generate random numbers in Python, you need to import command as

```
import random

random.random()
```
This returns a random floating point number in the range [0,1)

### 31) Explain how can you access a module written in Python from C?

You can access a module written in Python from C by following method,
```
Module = =PyImport_ImportModule("<modulename>");
```
### 32) Mention the use of ```//``` operator in Python?

It is a Floor Divisionoperator , which is used for dividing two operands with the result as quotient showing only digits before the decimal point. For instance, ```10//5 = 2``` and ```10.0//5.0 = 2.0```.

### 33) Mention five benefits of using Python?

* Python comprises of a huge standard library for most Internet platforms like Email, HTML, etc.
* Python does not require explicit memory management as the interpreter itself allocates the memory to new variables and free them automatically
* Provide easy readability due to use of square brackets
* Easy-to-learn for beginners
* Having the built-in data types saves programming time and effort from declaring variables

### 34) Mention the use of the split function in Python?

The use of the split function in Python is that it breaks a string into shorter strings using the defined separator. It gives a list of all words present in the string.
