# 25 Python Interview Questions

**1. What is Python? What are the advantages of using Python?**

Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation.

**2. What is a dynamically typed programming language?**

In dynamically typed programming languages, type checking is performed at runtime. This means that variables are checked against types only when the program is executing and also that the type of a variable is allowed to change over its lifetime.

Examples: ```Python, JavaScript, Lisp, PHP, Ruby, Perl, Lua```

**3. What is an interpreted programming language?**

An interpreted language is a programming language that is generally interpreted, without compiling a program into machine instructions. It is one where the instructions are not directly executed by the target machine, but instead, read and executed by some other program.

Examples: ```JavaScript, Perl, Python, BASIC```

**4. What is PEP 8 and why is it important?**

Introduced in 2001, PEP 8 is a document that provides guidelines and best practices on how to write Python code. The primary focus of PEP 8 is to improve the readability and consistency of Python code.  
PEP stands for Python Enhancement Proposal, and there are several of them. A PEP is a document that describes new features proposed for Python and documents aspects of Python, like design and style, for the community.

**5. What is Scope in Python?**

A variable is only available from inside the region it is created. This is called scope.  
A variable created inside a function belongs to the local scope of that function, and can only be used inside that function.  
A variable created in the main body of the Python code is a global variable and belongs to the global scope. Global variables are available from within any scope, global and local.

**6. What are lists, tuples and sets? What is the key difference between them?**

Lists, tuples and sets are used to store multiple items in a single variable.  
A list is a collection which is ordered, changeable, indexed and allows duplicate members.  
A tuple is a collection which is ordered, unchangeable, indexed and allows duplicate members.  
A set is a collection which is unordered, unchangeable*, unindexed and duplicate members are not allowed. *Set items are unchangeable, but you can remove and/or add items whenever you like.

**7. What are the common built-in data types in Python?**

In programming, data type is an important concept. Variables can store data of different types, and different types can do different things. Python has the following data types built-in by default, in these categories:

* Text Type: ```str```
* Numeric Types: ```int, float, complex```
* Sequence Types: ```list, tuple, range```
* Mapping Type: ```dict```
* Set Types: ```set, frozenset```
* Boolean Type: ```bool```
* Binary Types: ```bytes, bytearray, memoryview```
* None Type: ```NoneType```

**8. What is ```pass``` in Python?**

The ```pass``` statement is used as a placeholder for future code.  
When the ```pass``` statement is executed, nothing happens, but you avoid getting an error when empty code is not allowed.  
Empty code is not allowed in loops, function definitions, class definitions, or in if statements.

**9. What is the main() function in Python?**

In Python the ```main()``` function is the entry point of the program. The Python interpreter executes the from the first line of the program and it goes line by line.
So in conclusion Python doesn't have a ```main()``` function or it is considered to be the current module.

Workaround:

```python
# This will be executed when the current module is imported
# because it is outside our function
print("Hi there!")

# This will not be executed when the module is imported
# because it is just a function definition
# a function runs when it is called
def hello():
    print("Hello World!")

# If we want to run the hello() function
# we can use the following statement
if __name__ == '__main__':
    hello()

# because Python assigns the name '__main__' to the current module when it is executed directly
# but not when it is imported

# __name__ is a special variable, it is the name Python assigns automatically to the current module
```

**10. What are public, protected and private variables in Python?**

All members of a class are by default ```public``` in Python. These members can be accessed outside of the class, and their values can be modified too.  
  
```protected``` members of a class can be accessed by other members within the class and are also available to their subclasses.  
  
The ```private``` members of a class are only accessible within the class. In Python, a private member can be defined by using a prefix __ (double underscore).

**11. What is the use of ```self``` in Python?**

```self``` represents the instance of the class. By using the "self"  we can access the attributes and methods of the class in python. It binds the attributes with the given arguments.

**12. What is ```__init__``` in Python?**

```__init__``` is a reserved method in python classes. It is known as a constructor in object oriented concepts. This method called when an object is created from the class and it allow the class to initialize the attributes of a class.

**13. What is ```break``` and ```continue``` in Python?**

The ```break``` keyword is used to break out a ```for``` loop, or a ```while``` loop.  
  
The ```continue``` keyword is used to end the current iteration in a ```for``` loop (or a ```while``` loop), and continues to the next iteration.

**14. What is a unit test in Python?**

A unit test is a test that checks a single component of code, usually modularized as a function, and ensures that it performs as expected. Unit tests are an important part of regression testing to ensure that the code still functions as expected after making changes to the code and helps ensure code stability.

**15. What is docstring in Python?**

Python docstrings are the string literals that appear right after the definition of a function, method, class, or module.

**16. What is slicing in Python?**

Slicing in Python is a feature that enables accessing parts of sequences like *strings*, *tuples*, and *lists*. You can also use them to modify or delete the items of mutable sequences such as *lists*.

**17. What is the difference between Python arrays and lists?**

Lists and arrays behave similarly. Just like arrays, lists are an ordered sequence of elements. They are also mutable and not fixed in size, which means they can grow and shrink throughout the life of the program. Items can be added and removed, making them very flexible to work with.  
  
Lists store items that are of various data types. This means that a list can contain integers, floating point numbers, strings, or any other Python data type, at the same time.  
  
Arrays store only items that are of the same single data type. There are arrays that contain only integers, or only floating point numbers for example.

**18. How is memory managed in Python?**

**19. What are Python namespaces? Why are they used?**

**20. What is Scope Resolution in Python?**

**21. What are decorators in Python?**

**22. What are Dict and List comprehensions?**

**23. What is the ```lambda``` function? Why is it used?**

**24. How do you copy and object in Python?**

**25. What is the difference between ```xrange``` and ```range``` in Python?**

## More Questions

**What is a statically typed programming language?**

In statically typed languages, type checking is performed during compile time. It means that the type of a variable is known at compile time. Variables generally are not allowed to change types. For some languages, the programmer must specify what type each variable is, other languages offer some form of type inference.

Examples: ```C, C++, Java, Scala, Haskell```

**What is an compiled programming language?**

A compiled language is a programming language that is generally compiled and not interpreted. It is one where the program, once compiled, is expressed in the instructions of the target machine; this machine code is undecipherable by humans.

Examples: ```C, C++, C#, COBOL, Java```

**What is the difference between a high-level and a low-level programming language?**

The main difference between high-level language and low-level language is that, Programmers can easily understand or interpret or compile the high level language in comparison of machine. On the other hand, Machine can easily understand the low level language in comparison of human beings.

High-level: ```Python, Java, C#, JavaScript```

Low-level: ```Rust, Fortran, x86 Assembly, COBOL```

In the old days, C was considered a high-level language. Nowadays C and C++ are considered low-level languages because they have no automatic memory management.

## Work in progress...
