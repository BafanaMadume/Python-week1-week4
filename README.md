# Python-week1-week4
# WEEK-1
### JUPYTER NOTES
Run command on command Prompt =Type "jupyter notebook" in the command prompt.
#### SHORT CUTS ON JUPYTER
* New Cells = SHIFT+ENTER
* Deleting Cells = click outside cell to turn on command mode.then type dd
* To add a cell above or below an existing cell try making use of A and B as short cuts 
* Markdown cells= pressing M in command mode(ask question of how do i gop to command mode),another method of commentng as # is using CTRL+?

# PYTHON NOTES
This is a brief summary of important information that relates to python,ranging from python syntax and data types ,python functions and modules,python data structures and algorithms ,python for data analysis and visualization ,python for web developmnt and machine learning.in python python syntax can be executed by writing directly in the command line,or by creating a python filr on the server using .py file extension

* Comments in python start with a HASH #

# VARIABLES AND TYPES
Note python has no command for declaring a variable,and a variable is created the moment you assign a value to it.
### Variables rules
* A variable name must start with a letter or the underscore character
* A variable name cannot start with a number
* A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
* Variable names are case-sensitive,
#### variable names techniques
*  Camel Case = myVariableName,
*   Pascal Case = MyVariableName,
*   Snake Case = my_variable_name
* A variable name can include upper and lower case letters as well as underscores,but it will traditionally begin with lowercase letters 
  
types of variables ; integers ,whole number.Floats ,which are decimal numbers,complex numbers 
strings are normally collections of different characters
Booleans,are true or false values.
* in order to concatenate strings we use a + sign.please note that that + can not be used .
Example 
x = 4        # is an int
x = "Bafana"  # this becomes a string

## DATA STRUCTURES
Data structures allows for the storage of a list of values in a single variaber
 #### list []
Is a data structure which can contain any data type,including a list within a list.
* Set is also similar to a list but only difference is that it only contains unique elements and is declared using curly braces
* duplicates are allowed
* Example
* my_list = [[1,2,3],[False,True],[]]
print(my_list);

#### Sets {}
Set items are uchangeable ,but you can remove and add new items ,Sets are used to multipl e items in a single variable
* Duplicates are not allowed in a set
* more efficiently in memory ,like X Y coordinate pairs
* Example
* my_set={1,2,3,4,""}
print(my_set);

#### Dictionaries
Dictionaries are declared using curly braces nd can be accessed using keys

### SUMMARY of Data Structures
Python Collections (Arrays)
There are four collection data types in the Python programming language:

* List is a collection which is ordered and changeable. Allows duplicate members.
* Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
* Set is a collection which is unordered, unchangeable*, and unindexed. No duplicate members.
* Dictionary is a collection which is ordered** and changeable. No duplicate members



# OPERATORS 
operators are instructions that perform operations on variables and values in python,operators are used to perform and manipulate actions on data,

## Arithmetic operators
* Addition = +
* Subtraction = -
* Multiplication = *
* Division = /
* Modulus = %
* Exponentiation = **
* Floor division = //

## Comparison Operators
comparision operators evaluate two variables or values and then produce a Boolean Result either a True or false 
* Equal = ==
* not equal = !=
* Greater than = >
* Less than = <
* Greater than or equal to = >=
* less than or equal to = <=

## Logical Operators
They operator on boolean values and are used to combine conditional statements

* And = Returns True if both statements are true
* OR = Returns True if one of the statements is true
* Not = Reverse the result ,returns false if the result is true basically it negates the boolean value it operates on 

## Membership Operators
* in = Returns True if a sequence with the specified value is present in the object
* not in = Returns True if a sequence with the specified value is not present in the object

# CONTROL FLOW
1. IF STATEMENT = if allows one to execute a block of code only if a certain condition is met. e.g a= True if a: print it is true
so if the  condition is met and is true the code indented will be executed ,so more code can be added by indenting the code under the if statement,if you add an else statement,the code under that will be executed if the condition is false

2. For Loop = a for loop can be used to iterate over a list or any iterable object(this is either a list,a tuple,a dictionary,a set,or a string)
   
3. While loop this keeps looping till it finds a condition that is false,e.g a=0 while a <5: print a,a=a+1.

# FUNCTIONS
python fuctions can be defined using the def keyword followed by the function name and also arguments which need to be in parentheses ,FUNCTION BODY is indented and contains the code that performs the desired operation on the inputs and the "RETURN" keyword is used to specify the output 

def my_function():
    print("hello from a function")
for calling the function use the function name followed by the parenthesis for example ,my_function()
* functions also emcompass arguments  whereby information can be passed into functions as arguments ,so arguments are specified after the function name inside the parentheses

# Classes and objects
A class is like an object contructor, or a blueprint for creating objects.
we use an uppercase letter for the class name, and we start defining all the functions and attributes inside the class definition

All classes have a function called __init__(), which is always executed when the class is being initiated.
Use the __init__() function to assign values to object properties, or other operations that are necessary to do when the object is being created:
The __str__() function controls what should be returned when the class object is represented as a string.
