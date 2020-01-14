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
