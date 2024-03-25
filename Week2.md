# Python Week2
## PYTHON FUNDAMENTALS
---


# 1. BASIC FUNCTION
function is a block of code which only runs when it's called,
* You can pass data ,which is known as parameters,into a function and the function can return data as a result

## Arguments
so when information is passed into functions ,it is passed as arguments.
* Arguments are specified after the function name,inside the parentheses ,one can add as many arguments as you want,just separate them with a comma.
* Arguments are shortened to **args** in python documentations

* Number of Arguments must be called with the correct number of arguments.,so if my function expects 2 arguments ,you have to call the function with 2 arguments not more not less

* A parameter is variable listed inside the parentheses in the function definition
* An argument is the value that is sent to the function when it is called
  
  ## ARBITARY ARGUMENTS, *args
  So if i don't know how many arguments that will be passed into your function we add *     before the parameter name in the function definition.
  * This way the function will receive a ***~tuple of arguments~*** and can access the items accordingly
  * Arbitrary Arguments are often shortened to *args in python documentations

## Keyword Arguments
*send arguments with key = value syntax 

## ARBITRARY KEYWORD ARGUMENTS , **kwargs

*  If we don't know how many keyword arguments that will be passed into your function,add two asterisk :** before the parameter name in the function definition.
*  This way  the function will receive a ***~dictionary of arguments~*** and can access the items accordingly.

# Default Parameter Value
how to use a default parameter value,so if we call function without argument ,it uses a default value.

# Passing a List as an Argument
* You can send any data types of argument to a function(string,number,list,dictionary etc), it will  be treated as the same data type inside the function.
* **If you send a list as an argument ,it will still be a list when it reaches the function:**

## 1.1 Anatomy of a Function
* Functions are composed of a name and parameters,they are denoted by a **def** statement

  ### Return Values
  * To let a function return a value ,use the return statement

  ### Pass Statement
  * function definitions cannot be empty ,if by chance we have a function definition with no content ,put in the pass statement to avoid getting an error.
---

## 1.2 VARIABLES AND SCOPE
This is how global and local variables interact in python .

#### Function Scope
This allowed us to see a tuple and dictionary of the passed arguments ,Another method allows us to access all variables with a python function without any aserisks.This method is called the **"locals"** function

##### LOCALS()
a variable that is created inside a function belongs to the local scope of that function,and can only be used inside that function
* Variable names that are only accessible locally within the function

##### GLOBAL()
A variable created in the main body of the python code is a global variable and beongs to the global scope .
* Global variables are available from within any scope,global and local
* A variable created outside of a function is global and can be used by anyone

## Function As Variables
### Variables as function
* Variables and function both have names and data associated with them .but for functions ,this data includes information about required parameters and the lines of instruction to be executed
* **A function is represented as an object in python**

  ## Viewing Function data with _code_
  * "code" attribute of python function objects can be used to confirm that functions are just variables in python.

  ## Text Processing in Python
  We have two text processing operations ,and a function that can make the text lowercase,
  remove punctuation ,new lines ,and words that are three characters or less,it can also  remove

## Lambda Functions
It is a small anonymous function.It can take any number of arguments,but can only have one expression

***syntax = lambda arguments : expression***
* lambda functions can come handy when you need to pass a function as an argument to another python function ,such as the sorted function that sorts a list of values.

  ### Reason we use lambda
  power of lambda is better shown when you use thm as an anonymous function inside another function.
  
---
# 2. CLASSES AND OBJECTS FUNDAMENTALS
Python is an object oriented language ,almost everything i python is an object,with its properties and methods .

Class is like an object constructor or a "blueprint" for creating objects
## CREATE A CLASS
To create a class use the keyword ```class```:

### The_init_()Function
this is executed when the class is being initiatedm we use the _init_() function to assign values to object properties or other operations that are necessary to do when the object is being created:

## Instance Attributes
so this is where we have two instance attributes such as name and legs,these are attributes that every instance of the dog classes possesses.so when we name a class rover we can print rover its name and legs using my.dog.name and my.dog.legs respectively

## Static Attributes
so instead of keeping it in the constructor,we deine it as a static variable outside of the constructor.

---
# 3. ERROR HANDLING FUNDAMENTALS
---
# 4. THREADS AND PROCESSES FUNDAMENTALS
---
# 5. FUNDAMENTALS OF WORKING WITH FILES
---
