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
  * function definitions cannot be empty ,if by chance we have a function definition with no content ,put in the pass statement to avoid getting an error
---
# 2. CLASSES AND OBJECTS FUNDAMENTALS
---
# 3. ERROR HANDLING FUNDAMENTALS
---
# 4. THREADS AND PROCESSES FUNDAMENTALS
---
# 5. FUNDAMENTALS OF WORKING WITH FILES
---
