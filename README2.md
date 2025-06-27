# 25_python_interview_questions

**1. What is Python? What are the advantages of using Python?**

Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation.

---

**2. What is a dynamically typed programming language?**

In dynamically typed programming languages, type checking is performed at runtime. This means that variables are checked against types only when the program is executing and that the type of a variable can change over its lifetime.

Examples: `Python, JavaScript, Lisp, PHP, Ruby, Perl, Lua`

---

**3. What is an interpreted programming language?**

An interpreted language is a programming language where instructions are executed by another program (an interpreter) rather than compiled directly into machine code beforehand.

Examples: `JavaScript, Perl, Python, BASIC`

---

**4. What is PEP 8 and why is it important?**

Introduced in 2001, PEP 8 is a style guide for Python code that promotes readability and consistency.  
PEP stands for Python Enhancement Proposal — a design document providing information to the Python community.

---

**5. What is Scope in Python?**

Scope defines the visibility and lifetime of variables.  
- Variables created inside a function have local scope and are accessible only within that function.  
- Variables created in the main body have global scope and are accessible throughout the program, including inside functions (unless shadowed).

---

**6. What are lists, tuples, and sets? What is the key difference between them?**

Lists, tuples, and sets are collections used to store multiple items in a single variable.

- **List**: Ordered, mutable, indexed, allows duplicates.  
- **Tuple**: Ordered, immutable, indexed, allows duplicates.  
- **Set**: Unordered, mutable (you can add/remove items), unindexed, no duplicates allowed.  
  *Note: Set items themselves are immutable.*

---

**7. What are the common built-in data types in Python?**

Python includes these built-in data types:

- **Text Type**: `str`  
- **Numeric Types**: `int`, `float`, `complex`  
- **Sequence Types**: `list`, `tuple`, `range`  
- **Mapping Type**: `dict`  
- **Set Types**: `set`, `frozenset`  
- **Boolean Type**: `bool`  
- **Binary Types**: `bytes`, `bytearray`, `memoryview`  
- **None Type**: `NoneType`

---

**8. What is `pass` in Python?**

The `pass` statement is a no-operation placeholder used when a statement is syntactically required but no action is needed.

- Prevents syntax errors in empty blocks such as loops, function definitions, classes, or conditionals.
- Executes without doing anything.

---

**9. What is the main() function in Python?**

Python does not have a built-in `main()` function like some other languages. The interpreter runs the script from the top line down, executing all top-level code.

To simulate a `main()` entry point, the common pattern is:

```python
# This runs on import, since it's top-level code
print("Hi there!")

def hello():
    print("Hello World!")

# This runs only if the script is executed directly, not when imported
if __name__ == '__main__':
    hello()

---

**10. What are public, protected and private variables in Python?**

- **Public** members are accessible from anywhere — inside or outside the class.  
- **Protected** members (by convention) use a single underscore prefix `_` and are intended for internal use within the class and subclasses.  
- **Private** members use a double underscore prefix `__` and are name-mangled to be accessible only within the class.

---

**11. What is the use of `self` in Python?**

`self` represents the instance of the class. It allows access to instance attributes and methods, binding them to the current object.

---

**12. What is `__init__` in Python?**

`__init__` is the constructor method called automatically when an object is instantiated. It initializes the object's attributes.

---

**13. What is `break` and `continue` in Python?**

- `break` exits the nearest enclosing loop immediately.  
- `continue` skips the rest of the current loop iteration and proceeds to the next iteration.
