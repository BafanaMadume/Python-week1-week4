# python 

1.Variables and types
2 data structures
3.operators
4.control flow
5. function introduction
6.classes and objects intro

1.VARIABLES AND TYPES
* variables are fundamental building blocks in any programming language,they act like labeled containers that containers that store data for your program to manipulate
* variable name can include upper and lower case letters as well as underscores,variable name traditionally begin with lowercase in python
* We have several types of variables in python ,including integars ,which are whole numbers;floats which are decimal numbers ;complex numbers which are used for mathematical calculations

# 1. DATA TYPES
Data types in python define the kind of data a variable can hold.They determine how python interprets and uses the value stored in the variable

## 1.1 NUMERIC TYPES
* **integars`(int)`**= represent whole numbers ,positive,negative ,or zero `(e.g . 10,-5 , 0)`
* **Floating-point Numbers `(float)`**:These represent numbers with decimal points `(e.g , 3.14,-12.5)`
* python automatically returns a float to accommodate non-whole numbers.adding a float to an int or multiplying or using exponents with both also returns a float
* - pitfall of floats is that they are approximations,which can result in rounding errors
  - e.g 1.2 minus 1.0 equals 0.1999999999996 instead of 0.2.
  - floats are stored as binary ones and zeros in memory and due to limited memory,floating point errors that can be problematic in certain situations such as when dealing with money.
* To use the decimal module you need to import the decimal class and the getcontext function at the top of your code.
* getcontext() function returns a context object that holds global settings for using the decimal class.

## 1.2 String Type `(str)`:
* Strings represent sequences of characters including letters,numbers,symbols ,and spaces.They are enclosed in single `(')` or double`(")` quotes.`(e.g , "Hello,world",'This is a string')`
* Slicing refers to taking a portion of a string and returning it.
* **f string** allow us to insert variables or expressions inside curly braces in a string
* f strings can also do rounding and number formatting,they provide a more concise and convenient alternative to traditional string formatting methods like .format() method and the modulo operator().
## Here's how f-strings work:

* **Prefix**:  An f-string is created by prefixing a string literal with the letter f or F (case-insensitive).

* **Expressions within Curly Braces**:  Inside the f-string, you can embed expressions enclosed in curly braces {}. These expressions can be variables, function calls, calculations, or any valid Python expression.

* **Evaluation and Insertion**:  When the f-string is evaluated, the expressions within curly braces are evaluated first. The resulting values are then inserted directly into the string at their respective positions.

## Benefits of F-strings:

1.**Readability:** F-strings make code more readable because you can directly include variable names and expressions within the string itself. This improves code clarity compared to other formatting methods.
2.**Conciseness:** F-strings eliminate the need for extra formatting syntax like .format() method calls or string concatenation with +.
3.**Flexibility:** You can include complex expressions and formatting options within the curly braces, providing more control over the final output.

### Slicing
* it is a powerful technique for extracting substrings from a string.it allows you to grab a specfic portion of characters without modifying the original string
* `syntax = new_string = original_string[start:end:step]`
* **start (optional)**: The index of the first character to include in the slice (defaults to 0, which refers to the first character).
* **end (optional)**: The index of the first character not to include in the slice (up to, but not including that character).
* **step (optional)**: The step size to take while extracting characters. Defaults to 1 (extracts every character).


## 1.3 Boolean Type `(bool)`:
* Booleans represent logical values: True and False.They are used for conditional statements and other logic -based operations `(eg True,False)`

## 1.4 BYTES
Bytes represent a sequence of integers ranging from 0 to 255. They are fundamental for working with binary data, which is the raw form of information processed by computers.
* Binary Data : Computers store and process information in binary format using bits (0s and 1s),bytes are a way to group these bits together
* Not Text : Bytes are distinct from text data (strings)

In programming languages like Python, operators are symbols that perform operations on values. They can be categorized into different types based on their function:

* **Arithmetic Operators:** Perform basic mathematical calculations like addition (`+`), subtraction (`-`), multiplication (`*`), division (`/`), floor division (`//` - integer result), modulo (`%` - remainder).
* **Comparison Operators:** Compare values and return boolean results (True or False). Examples include `==` (equal to), `!=` (not equal to), `<` (less than), `>` (greater than), `<=` (less than or equal to), `>=` (greater than or equal to).
* **Logical Operators:** Combine boolean expressions. Include `and` (both conditions true), `or` (at least one condition true), `not` (inverts the truth value).
* **Assignment Operators:** Assign values to variables. The basic assignment is `=`, but there are also combined assignment operators like `+=` (add and assign), `-=` (subtract and assign), etc.
* **Membership Operators:** Check if a value exists within a sequence (like a list). Examples include `in` (checks if a value is present) and `not in` (checks if a value is not present).
* **Identity Operators:** Compare the memory location of objects. These are `is` (checks if objects are the same object) and `is not` (checks if objects are different objects).
 

  Question and Answer
* 1. What is the value of int('101', 2)? = 5
* 2. What is the value of int(8.7)? = 8
* 3. What is the value of this statement? bool(-1) == 1 = True
* 4. What class might be used to store precise monetary amounts for a banking application? = decimal
* 5. What does bytes(4) do? = It creates an empty bytes object 4 bytes long

---

2. DATA STRUCTURES
   2.1 Lists
   2.2 Tuples
   2.3 Sets
   2.4 Dictionaries

# 2.1. LIST `[]` 
* **O**rdered
* **C**hangeable
* **A**llow duplicates values

  - We use SQUARE BRACKETS `[]`: Lists are enclosed in square brackets .i separate items within the brackets with commas
  - list items are indexed ,the first item has index[0],the second item has index [1]

### Common List Methods

* ``append()``:add an element at the end of the list
* ``insert()``:insert an element at a specific index
* ``remove()``: Remove the first occurence of a value from the list
* ``pop()``: Remove and return the element at a specific index(defaults to the last
* ``extend()``= extend the list by appending all the items froman iterable
* ``sort()``: Sort the list items in place(ascending order by default)
* ``copy()``

# 2.2 Tuples `()`
* **O**rdered
* **U**nchangeable =ideal for situations where you need data integrity and want to prevent accidental changes
* **A**llow duplicates

### Common Tuple Methods
* ``Count()`` = count the number of occurence of a value within a tuple
* ``index()`` = Find the index of the first occurrence of a value
* ``len(tuple)`` = Get the length (number of elements) of the tuple

* They provide data integrity and are efficient for small frequently accessed data
* use them when you don't need to modify the content after creation.

## 2.3 SETS `{}`
* **U**nordered
* **U**nchangeable
* **U**nindexed
* **N**o duplicates

  
they offer a unique way to store and manipulate collections of items .sets focus on uniqueness rather than maintain order 
* Curly braces : sets arew enclosed in curly braces {},and the elements within the braces are separated by commas

## 2.4 Dictionaries
theyn are often called associative,are fundamental data structures in python .they store data in a key-value format

1. creating dictionaries:
   curly braces {} dictionaries are enclosed in curly braces{} and items within curly braces consist of a key followed by a colon(:) and then its corresponding value.

## Common dictionary Methods
* **get(key,default)**=Retrieves the value for a key. If the key doesn't exist, you can optionally provide a default value to return
* **keys()**= Returns a view of all the keys in the dictionary as a set
* **values()**=Returns a view of all the values in the dictionary as a list.
* **items()**=Returns a view of all key-value pairs in the dictionary as tuples.
* **pop()**=Removes the key-value pair with the specified key and returns its value. If the key doesn't exist, you can optionally provide a default value.
* **update()**=Updates the dictionary by adding key-value pairs from another dictionary (can overwrite existing keys).

### WHEN TO USE DICTIONARIES
* **Storing key-value pairs** = use dictionaries whenever you need to associate unique keys with data or information ,such as user profiles (username:"alice", email:"[email address removed]"
* **fast lookups**=Accessing elements by key is very efficient in dictionaries, making them ideal for scenarios where you need to retrieve data based on a unique identifier.

Dictionaries effectively, you can create well-structured and organized data representations in your Python programs

# 3 CONTROL FLOW
it refers to how your program executes instructions in a specific order .it determines the sequence in which the code is evaluated allowing you to make  decisions.repeat actions and structure your program's logic

## CONDITIONAL STATEMENTS

* ``if`` statements allows you to executr code blocks only when a certain condition is true
* ``Elif`` else if way of saying that if the previous conditions were not true then try this condition

---
# MOCK QUESTIONS
## Data types
1.Which of the following data types can hold a decimal number in Python?
- a) int
- b) **``float``**
- c) string
- d) bool

2. A variable in Python can store different data types throughout the program. (True/False)
- a) **``True``**
- b) False

3.What data type is commonly used to represent text in Python?

- a) number
- b) character
- c) **``string``**
- d) text

4.Which data type can hold a logical value (True or False)?

- a) decimal
- b) boolean
- c) logical
- d) **``bool``**

5.How can you represent a collection of items of different data types in Python?

- a) Single string with comma separation
- b) Special collection data type
- c) **``List ([])``**
- d) Tuple (())
---

## Data structures
6.Which data structure is most efficient for checking if an element exists in a collection?
- a) list
- b) tuple
- c) **``set``**
- d) dictionary

7.Ordered collections of items that can be modified after creation are called:
- a) **``lists``**
- b) tuples
- c) sets
- d) dictionaries

8.What is the key difference between a list and a tuple in Python?
- a) Tuples can hold different data types, while lists cannot.
- b) **``Lists are mutable, while tuples are immutable``**.
- c) Tuples can store elements by reference, while lists store by value.
- d) Lists are faster for accessing elements by index, while tuples are slower.
  
9.What data structure would you use to store unique elements and efficiently check if an element exists in the collection?

- a) list
- b) tuple (unchangeable order)
- c)**``set``**
- d) dictionary

## Control Flow

6.Which control flow statement allows you to repeat a block of code as long as a condition is true?
- a) if
- b) elif
- c) for
- d)**``while``**

7.What is the correct way to define a function in Python?
- a) **``def function_name(arguments): (code block)``**
- b) function_name(arguments) = (code block)
- c) func function_name(arguments): (code block)
- d) function_name: (arguments) -> (code block)

8.In Python, indentation is used for: (Select all that apply)
- a) **``Defining code blocks within control flow structures (if, loops)``**
- b) **``Improving readability of code``**
- c) Specifying variable data types
- d) Separating function arguments


10. What is the correct syntax for a basic `if` statement in Python?
    * a) **``if condition: (code block)``**
    * b) when condition: do (code block)
    * c) if (condition) {code block}
    * d) check condition: (code block)

11. How can you execute a block of code only if a specific condition is not met (the opposite of(if)?
    * a) **``Use else with the if statement: if condition: (code block) else: (alternate code block)``**
    * b) Utilize the unless keyword (not a built-in keyword in Python)
    * c) Define a separate function for the alternate scenario.
    * d) Indent the code block outside of the if statement.

12. What is the purpose of the `elif` statement in Python?
    * a) **``To define an alternative condition within an if statement if the first condition is False.```**
    * b) To loop through a collection of items.
    * c) To terminate a loop prematurely.
    * d) To define a function with multiple arguments.

13. How can you iterate over a sequence of elements in Python, executing a code block for each element?
    * a) Use a while loop with a counter variable.
    * b) **``Employ a for loop with the element as the loop variable.``**
    * c) Call a built-in iterate function on the sequence.
    * d) Access elements by index and perform actions individually.

14. What is the difference between a for loop and a while loop in Python?
    * a) for loops are always faster than while loops.
    * b) **``for loops are designed for iterating over sequences, while while loops can be used for any condition.``**
    * c) while loops require an incrementing counter, while for loops don't.
    * d) for loops are only for strings, while while loops work with any data type.

15. What is the correct way to break out of a loop prematurely in Python?
    * a) Use the exit statement (can be dangerous for overall program flow).
    * b) Employ a conditional statement within the loop to modify the loop variable.
    * c) **``Utilize the break statement to exit the loop entirely.``**
    * d) Simply remove the loop condition.

16. How can you continue to the next iteration of a loop without executing the remaining code in the current iteration?
    * a) Modify the loop counter to skip the current iteration.
    * b) Utilize the `next` statement (not commonly used for loop control).
    * c) **``Employ the `continue` statement to skip to the next iteration.``**
    * d) Add a conditional statement to bypass specific code within the loop.
   
  ---
  ---
  ---

# WEEK 2 = PYTHON FUNDAMENTALS

- 1. Basic functions
- 2. classes and objects fundamentals
- 3. Error Handling Fundamentals
- 4. Threads and processes Fundamentals
- 5. Fundamentals of working with files
 

# FUNCTIONS
functions are composed of a name and parameters ,name and parameters are denoted by a def statement
* def function_name(arguments):
  
    """ Docstring (optional) """
  
      Function body (code to be executed)
  
  return output_value (optional)

  * def =  keyword to define a function.
  * function_name: a descriptive name for your function (follows variable naming conversions)
  * arguments : comma-separated list of variables that the function can accept as input (optional,can be empty parentheses()
  * function body = the indented block of code that dfines the functions logic and operations
  * return output value :a statement that specifies the value of the function a

## Advantages of Functions:

* Code Reusability: Functions allow you to write a piece of code once and use it multiple times throughout your program, reducing redundancy.
* Improved Readability: Functions break down complex logic into smaller, manageable blocks with clear names, enhancing code readability.
* Modularity: Functions promote modularity by grouping related code together, making the program easier to understand and maintain.

## NAMED PARAMETERS
also named arguments or keyword arguments ,are a way to pass arguments to a function by associating them with their parameter names during the function call
* named parameters are useful for function with many optional arguments or when the order of arguments might not be intuitive
* By understanding and using named parameters effectively, you can enhance the readability and maintainability of your Python code

### *ARGS
a rule when using keyword arguments in python ,they must come after the positional arguments.The order of the first two arguments
* args represent a tuple that collects all non keyword arguments passed to the function
* it allows you to accept an arbitrary number of positiopnal arguments beyond the defined parameters in the function signature
* *args captures all arguments as a tuple within the function.

### Kwargs 
* represent a dictionary that collects all keyword argumentd passed to the function
* it allows you to accept an arbitrary number of named arguments,providing more flexibilty in how arguments are passed

## WHEN TO USE args and kwargs
* use args when you expect a varying number of positional arguments and want to process them all
* use **kwargs 


In object-oriented programming (OOP), classes and objects are fundamental concepts that model real-world entities and their behaviors. Here's a breakdown of their relationship:

**1. Class:**

* A class is a blueprint or template that defines the properties (attributes) and functionalities (methods) that objects of a certain kind will share.
* It acts as a reusable specification for creating objects. 
* You can think of a class like a cookie cutter that defines the shape of cookies you can create.

**2. Object:**

* An object is an instance of a class. It's a concrete entity that represents a specific example of the class.
* An object has its own set of attributes (data) that hold specific values for that particular instance.
* It can also access and execute the methods defined in the class.
* Just like baking cookies from the cookie cutter, you can create multiple objects from a single class.

**Analogy:**

Imagine a class called `Dog`. This class might define attributes like `breed`, `name`, and `age`. It could also define methods like `bark()` and `play()`. An object of the `Dog` class, named "Fido", would be a specific dog with its own breed (e.g., "Labrador"), name ("Fido"), and age (e.g., 2). Fido could then use the `bark()` and `play()` methods inherited from the `Dog` class.

**Key Points:**

* A class defines the general structure, while an object is a specific instance with its own data.
* Objects can interact with each other by calling methods on each other.
* Classes promote code reusability and modularity.

**Example in Python:**

```python
class Car:
  """A simple Car class."""
  def __init__(self, make, model, year):  # Constructor (special method for initializing objects)
    self.make = make  # Attributes (data) specific to each object
    self.model = model
    self.year = year

  def accelerate(self):
    """Simulates car acceleration."""
    print(f"The {self.make} {self.model} is accelerating!")

# Creating objects (instances) of the Car class
my_car = Car("Honda", "Civic", 2020)
friend_car = Car("Toyota", "Camry", 2018)

# Accessing attributes and calling methods
print(f"My car is a {my_car.make} {my_car.model} from {my_car.year}.")
my_car.accelerate()

print(f"Friend's car is a {friend_car.make} {friend_car.model} from {friend_car.year}.")
friend_car.accelerate()
```

Here's a summary of instance and static attributes in object-oriented programming:

**Instance Attributes:**

* **Definition:** Unique variables that belong to a specific object (instance) of a class.
* **Purpose:** Store data specific to that object, allowing objects of the same class to have different characteristics.
* **Creation:** Defined within the class's constructor (often `__init__` in Python) and assigned values during object initialization.
* **Example:** In a `Dog` class, `name`, `breed`, and `age` could be instance attributes, where each `Dog` object has its own unique name, breed, and age.

**Static Attributes:**

* **Definition:** Variables shared by all objects of a class.
* **Purpose:** Represent data or properties that are constant or common to all instances of the class.
* **Creation:** Defined outside the constructor, usually within the class body.
* **Example:** In a `Math` class, a static attribute `PI` could hold the value of pi (3.14...). All `Math` objects would share this constant value.

**Key Points:**

* Instance attributes provide individuality to objects within a class.
* Static attributes promote code reusability and consistency across the class.
* Use instance attributes when each object needs its own set of data.
* Use static attributes for constants or properties that apply to all objects without variation.

Here's a table summarizing the key differences:

| Feature                 | Instance Attribute | Static Attribute |
|-------------------------|--------------------|-----------------|
| Definition              | Unique variable per object | Shared variable by all objects |
| Purpose                  | Stores object-specific data  | Represents class-level constants or properties |
| Creation                 | Defined and assigned values within `__init__` | Defined outside `__init__` within the class body |
| Example (Dog class)     | `name`, `breed`, `age` | Could be `MAX_AGE` (fixed value for all dogs) |

Understanding both instance and static attributes is crucial for creating well-structured and efficient object-oriented programs.




Threads and processing are fundamental concepts related to how computer programs handle tasks and utilize system resources. Here's a breakdown of each:

**1. Processes:**

* A process is an instance of a computer program that is actively running. It represents the execution of a program with allocated system resources like memory, CPU time, and open files.
* A single program can have multiple processes running concurrently, each handling a specific task.
* Processes are typically independent units, meaning issues in one process won't directly crash other processes from the same program.
* The operating system manages processes and their resources.

**2. Threads:**

* A thread is a lighter-weight unit of execution within a process. It shares the same memory space and resources (like open files) with other threads within the same process.
* Multiple threads can run concurrently within a single process, allowing for the execution of multiple tasks seemingly "at the same time." (In reality, the CPU rapidly switches between threads, creating the illusion of parallelism.)
* Threads provide a way to achieve concurrency within a process, improving responsiveness and performance for certain tasks.
* While threads share memory, they may require synchronization mechanisms to avoid data race conditions (conflicting access to shared data).

**Analogy:**

Imagine a process like a restaurant. The entire restaurant operation (taking orders, cooking, serving) is the process. Threads would be like individual chefs within the kitchen. They can all work on different dishes (tasks) concurrently, but they share the same kitchen resources (ovens, utensils).

**3. Processing and Threads:**

* Multithreading allows a single process to handle multiple tasks seemingly simultaneously, improving the program's responsiveness and efficiency for certain scenarios.
* Threads are particularly useful for tasks that involve waiting (e.g., network requests, user input) or performing independent computations.
* While threads can improve performance, they add complexity due to the need for synchronization and potential race conditions.

**4. When to Use Threads:**

* Consider using threads when your program needs to perform multiple tasks that can be done concurrently without heavy data sharing.
* Threads can be beneficial for improving user experience by keeping the program responsive during wait operations.

**5. Key Differences:**

Here's a table summarizing the key differences between processes and threads:

| Feature                 | Process                         | Thread                        |
|-------------------------|---------------------------------|------------------------------|
| Definition              | Instance of a running program    | Unit of execution within a process |
| Resource Management     | Independent (own memory, CPU time) | Shared (shares memory with other threads in the process) |
| Creation/Termination    | More expensive                  | Less expensive                  |
| Communication            | Requires inter-process communication (IPC) | Can directly access shared memory (requires synchronization) |

**6. Conclusion:**

Understanding the concepts of processes and threads is crucial for developing efficient and responsive programs. Processes provide isolation and resource management, while threads enable concurrency within a process. Choosing between processes and threads depends on the specific needs of your program and the nature of the tasks involved. 

