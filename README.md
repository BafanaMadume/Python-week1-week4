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

## def my_function():
    print("hello from a function")
for calling the function use the function name followed by the parenthesis for example ,my_function()
* functions also emcompass arguments  whereby information can be passed into functions as arguments ,so arguments are specified after the function name inside the parentheses

# Classes and objects
A class is like an object contructor, or a blueprint for creating objects.
we use an uppercase letter for the class name, and we start defining all the functions and attributes inside the class definition

All classes have a function called __init__(), which is always executed when the class is being initiated.
Use the __init__() function to assign values to object properties, or other operations that are necessary to do when the object is being created:
The __str__() function controls what should be returned when the class object is represented as a string.

# 1 BASIC DATA TYPES
* Text Type = str 
* Numeric Types = int ,float, complex
* Sequence Types = list,tuple ,range
* Mapping = dict
* Set types = set .frozenset
* Boolean Type = bool
* Binary Types = bytes, bytearray,memoryview
* None Type= NoneType

  ## Example of each data type 
  * x = "Hello World"                         = str
  * x = 20                                    = int
  * x = 20.5                                  = float
  * x = ij                                    = complex
  * x = ["apple","banana","cherry"]           = list
  * x = ("apple","banana", "cherry")          = tuple
  * x = range(6)                              = range
  * x = {"name":"john","age":36}              = dict
  * x = {"apple","banana","cherry"}           = set
  * x = frozenset({"apple","banana","cherry"} = frozenset
  * x = True                                  = bool
  * x = b"Hello"                              = bytes
  * x = bytearray(5)                          = bytearray
  * x = memoryview(bytes(5))                  = memoryview
  * x = None                                  = None

## 1.1 INTS AND FLOATS
int or integer is a whole number ,positive or negative without decimals of unlimited length
float or floating point number is a number,that is positive or negative and it contains one or more decimals.
*  x = 20                                    = int
*  x = 20.5                                  = float

## 1.2. BOOLEANS 
booleans simply refers to True and False 

### CASTING BOOLEANS
integers can be used as booleans where by:
0 =  False
1 = true

## 1.3. STRINGS
Slicng refers to taking a portion of a string and returning it,
* assinging a string to a variable is done with the variable name followed by an equal sign and the string
##### EXAMPLE AND SYNTAX

###### SLICING
name = "MY name is Bafana Gift Madume "

* name[0] = 'M'
* name[0:7] = 'MY name'
* name[11:30] = 'Bafana Gift Madume '

###### FORMATING 
F-String allow us to insert variables or expressions inside curly braces in a string

* 'My number is:'+str(5) = output = 'My number is:5'
* f'My number is:(5)' = using the f string

###### MULTI_LINE STRINGS
This is a feature for creating a  multiline string using triple quotes,
if i want ot include triple quotes in the string we can escape them with a backlash

## 1.4. Bytes
This is the data passed around but rarely modifies directly,one can use byte array if you need to midift the data.one can treat byte array like a string and modify specific byte values using slice notation

# 2 BASIC DATA STRUCTURE

## 1.1 LIST 
#### list slicing 
from this negative values can be used to step backward through the list,but all operations allow for the extraction of data from lists or strings one value at a time

* Examples
* myList = [1,2,3,4,5] = output = [4, 5]
  myList[3:]

* for i in range(10): OUTPUT=[0123456789]
    print(i)
* myList = list(range(100))
  - myList[::10] = [0, 10, 20, 30, 40, 50, 60, 70, 80, 90]
  - myList[::-10] = [99, 89, 79, 69, 59, 49, 39, 29, 19, 9]
 
#### Modifying list
* To add an item to the end of the list
  - Append()
* inserting an item at a specific position
  - insert()
* To remove items from a list based on its value and not its index
  -remove()

## Tuples()


## SETS


## DICTIONARIES
Dictionaries are mainly used to store data values in key:value pairs,it is a collection which is ordered ,changeable and do not allow duplicates ,They are written with curly brackets and the have keys and values

* **Examples**

-thisdict = {
  -  "brand":"ford",
  -  "model": "Mustang",
  -   "year" : 2020,
  -  "year" : 2023
- }

## ACCESSING ITEMS IN A DICTIONARY

 - thisdict = {
   - "brand":"Ford",
    -"model":"Mustang",
    -"year": 2020
-}
-x = thisdict["model"] # accessing what is required
- print(x) = mustang
- thisdict.get("model") # get is also a fast method to obtain what is required

  ### Keys()
  * x = thisdict.keys() #keys() method will return a list of all the keys in the dictionary

  ##### Adding  new item to the original dictionary
  * car = {
 - "brand":"Toyota",
 - "model":"Corolla",
 -"year" : 2024
-}

- x = car.keys()
- print(x)

- car["color"] = "white" # this is how you add a new key ot iten=m 

- print(x)
- dict_keys(['brand', 'model', 'year'])
- dict_keys(['brand', 'model', 'year', 'color'])

  ### items()
  this method will return each item in a dictionary ,as tuples in a list

  * x=thisdict.items()
- print(x)

#### Check if key exist
kindly refer to python file with code

### CHANGING VALUES
#### update()
update() method will update the dictionary with the items from the given argument.
The argument must be a dictionary, or an iterable object with key:value pairs.

### REMOVING ITEMS
*refer to jupyter for more clarify on notes and code*
* pop() = pop() method removes the item with the specified key name
* popitem() = The popitem() method removes the last inserted item
* del
* clear() =  method empties the dictionary

### COPY A DICTIONARY 
You cannot copy a dictionary simply by typing dict2 = dict1, because: dict2 will only be a reference to dict1, and changes made in dict1 will automatically also be made in dict2 ways to make a copy, one way is to use the built-in Dictionary method copy()
---
---
# LIST COMPREHENSION
it offers a s way shorter syntax when you want to create a new list based on the values of an existing list
  first list comprehension 
