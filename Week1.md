# Python-week1
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

## 2.1 LIST  [OCA]
1. **Ordered**
2. **Changeable**
3. **Allow duplicate values.**

* list items are indexed, the first item has index [0], the second item has index [1]

  #### list() = use this when creating a new list
---
* Example
  
thislist = list(("apple","banana","cherry"))

print(thislist)

---
### ACCESSING ITEMS ON LIST
***Example 1:***

**Print the second item of the list**

thislist=["apple","banana","cherry"] #the list

print(thislist[1])

= *banana*

---
### Negative indexing ,basically starting from the end¶
-1 refers to the last item, -2 refers to the second last item

***Example 2:***
**Print the last item of the list**

thislist = ["apple","banana","cherry"];

print(thislist[-1])

= *cherry*

---
### Range of indexes
where to start and where to end the range.

When specifying a range, the return value will be a new list with the specified items

***Example 3***
**Return the third, fourth, and fifth item**
            1st  ,   2nd   ,    3rd   ,    4th  ,    5th  ,    6th  ,    7th  item 
          
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]

            0    ,      1        

print(thislist[2:5])

---
# Check if Item Exists
***example 4***
**Check if "apple" is present in the list:**

thislist = ["apple", "banana", "cherry"]

if "apple" in thislist:

    print("yebo madala")

---
# CHANGE ITEM VALUE
***example5***
**Change the second item:**

thislist = ["apple","banana","cherry"]

thislist[2] = "grapes" use indexing

print(thislist)

# CHANGE A RANGE OF ITEM VALUES
***example8**
***Change the values "banana" and "cherry" with the values "blackcurrant" and "watermelon":**

print("oldlist")

thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"];

print(thislist)

print("newlist")

thislist[1:3]=["blackcurrant","watermelon"]

print(thislist)

= **output**
oldlist

['apple', 'banana', 'cherry', 'orange', 'kiwi', 'mango']

newlist

['apple', 'blackcurrant', 'watermelon', 'orange', 'kiwi', 'mango']

---
# Python - Add List Items
## APPEND ITEMS
THIS IS TO ADD AN ITEM TO THE END OF A LIST

**APPEND()**

**Example**

thislist=["apple","banana","cherry"]

thislist.append("grapes");

print(thislist)

## INSERT ITEMS
to insert item at a specified index

**insert()**

**Example**
**Insert an item as the second position**

thislist = ["apples","banana","cherry"];

thislist.insert(1,"grapes")

print(thislist)

---
## Extend List
append elements from another list to the current list
extend() method does not have to append lists, you can add any iterable object (tuples, sets, dictionaries 

**extend()**

**Example**

namelist = ["Bafana","Tyrone","Gift"]

surnamelist = ["Madume","Magadze","Baloyi"]

namelist.extend(surnamelist)

print(namelist)

= ['Bafana', 'Tyrone', 'Gift', 'Madume', 'Magadze', 'Baloyi']

---
## Remove List Items

**remove()**
method removes the specified item

***Remove "banana":***

thislist = ["banana","apple","avocado"]

thislist.remove("banana");

print(thislist)

## Remove Specified index

**pop()** method that removes the specified index

other option is 
**del**

**Example**
thislist = ["banana","apple","avocado"]

thislist.pop(0)

print(thislist)

---

## Loop Through the Index Numbers

loop through the list items by referring to their index number.

Use the **range()** and **len()** functions to create a suitable iterable

thislist = ["apples","banana","cherry"]

for i in range(len(thislist)):

    print(thislist[i])

---
# Python - Sort Lists

Sort List Alphanumerically

* List objects have a **sort()** method that will sort the list alphanumerical ascending, by default:

* Sort Descending To sort descending, use the keyword argument reverse = True:

# Copy a List

cannot copy a list simply by typing list2 = list1, because: list2 will only be a reference to list1, and changes made in list1 will automatically also be made in list2.

There are ways to make a copy, one way is to use the built-in List method copy()
* Another way to make a copy is to use the built-in method list()
  
**Example**
thislist = ["apple", "banana", "cherry"]

mylist = thislist.copy()

print(mylist)

---
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
---

# Tuples()
Tuple items are ordered, unchangeable, and allow duplicate values
* Ordered
* Unchangeable
* Allow duplicates
  
# Change Tuple Values
Once a tuple is created, you cannot change its values. Tuples are unchangeable, or immutable as it also is called.

 workaround. You can convert the tuple into a list, change the list, and convert the list back into a tuple

**Convert the tuple into a list to be able to change it:**

x = ("apple", "banana", "cherry")

y = list(x)

y[1] = "kiwi"

x = tuple(y)

print(x)

* tuples are unchangeable, so you cannot remove items from it, but you can use the same workaround as we used for changing and adding tuple items:

  **example**

  **Convert the tuple into a list, remove "apple", and convert it back into a tuple**

thistuple = ("apple", "banana", "cherry")

y = list(thistuple)

y.remove("apple")

thistuple = tuple(y)

---

## SETS{}
A set is a collection which is unordered, unchangeable*, and unindexed
* Note: Set items are unchangeable, but you can remove items and add new items.

* ***unordered***
* ***unchangeable***
* ***unindexed***


## DICTIONARIES

* ***ordered***
* ***changeable***
* ***do not allow duplicates***
  
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
  car = {
  
 "brand":"Toyota",
  
 "model":"Corolla",

 "year" : 2024
 
 }

 x = car.keys()
 
 print(x)
 
 car["color"] = "white" # this is how you add a new key ot iten=m

print(x)

dict_keys(['brand', 'model', 'year'])

dict_keys(['brand', 'model', 'year', 'color'])

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
it offers a way shorter syntax when you want to create a new list based on the values of an existing list.A list comprehension is enclosed in square brackets 
* list comprehension allows you to create a for loop in one line while also returning a copy of the list you're iterating over.it allows to enable filtering or applying funcctions to every item in a list
  first list comprehension 

**SYNTAX FOR LISt COMPREHENSION**

newlist = [expression ***for*** item ***in*** iterable ***if*** condition == True]

## example:

- myList = [1,2,3,4,5]
- [2 * item for item in myList]

* fruits =["apples" ,"banana","cherry","kiwi","mango"]
* newlist = [x for x in fruits if "a" in x]

  **SPLIT()**
  * This functions allows you to split a string based on a given character or string
 
    ---
    ---
    ---

# BASIC CONTROL FLOW 

Conditional statements 

python supports the usual logical conditions from math

* Equals : a == b
* not equals: a != b
* less than : a < b
* less than or equal to : a<=b
* greater than : a > b

  ## IF statement
  if the logical condtion is true,then the indented statement gets executed.if the logical condition is false,the indented statement is skipped
  * NB!! please pay close attention to indentation whitespace at the beginning of a line

  **Example**

- if x > 0:

    print(x is positive)

![if statement](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/b56e2823-ead1-40b8-b0d5-c8a6955537a6)


## if else statement
alternative execution in which two possibilities and the conditions determines which one is executed

![if else](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/23df3e44-4993-464c-88c9-5fb12a424506)


**Example** 
x =2

if x % 2 == 0:

   print("x is even")
   
else:

    print("x is odd")

***output*** = x is even 


## Elif (ELSE IF)
this is a way of saying that if the previous conditions were not true then try this condition.this is mostly based on the fact that sometimes there are more than two possibilities and we need more than two branches

***Example***
x = 1

y = 5

if x < y:

    print("x is less y")

elif(x > y):

   print("x is greater than y")

else:

   print("they are equal")


![else if](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/6a37cf34-05a7-4e11-aaab-6ece93eb8fa4)

![example and how syntax must flow](https://github.com/BafanaMadume/Python-week1-week4/assets/141032267/7092d40a-04b5-447f-81e1-2415c19649e1)
---
---
---

# WHILE 
With while loop we can execute a set of statements as long as a condition is true,
with the break statement we can stop the loop the loop even if the while condtion is true 

Break and continue can be used with the while

**example**

i = 1

while i < 6:

  print(i)
  
  i += 1

  output = 1,2,3,4,5

# FOR LOOP
it is used for iterating over a sequence ***(either a list ,tuple ,a dictionary ,a set ,or a string*** 

**Example**
fruits = ["apples","banana","cherry","grapes"]

for x in fruits:

    print(x)
* apples
- banana
- cherry
- grapes

for x in "banana":

    print(x)  
---

friends = ['joe','john','james']

for friend in friends: 

    print("merry christmas:",friend)
    
print("done")

output:
merry christmas: joe

merry christmas: john

merry christmas: james

done
