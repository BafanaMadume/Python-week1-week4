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

1. DATA TYPES
Data types in python define the kind of data a variable can hold.They determine how python interprets and uses the value stored in the variable

# 1.1 NUMERIC TYPES
* **integars`(int)`**= represent whole numbers ,positive,negative ,or zero `(e.g . 10,-5 , 0)`
* **Floating-point Numbers `(float)`**:These represent numbers with decimal points `(e.g , 3.14,-12.5)`
* python automatically returns a float to accommodate non-whole numbers.adding a float to an int or multiplying or using exponents with both also returns a float
* - pitfall of floats is that they are approximations,which can result in rounding errors
  - e.g 1.2 minus 1.0 equals 0.1999999999996 instead of 0.2.
  - floats are stored as binary ones and zeros in memory and due to limited memory,floating point errors that can be problematic in certain situations such as when dealing with money.
* To use the decimal module you need to import the decimal class and the getcontext function at the top of your code.
* getcontext() function returns a context object that holds global settings for using the decimal class.

# 1.2 String Type `(str)`
* Strings represent sequences of characters including letters,numbers,symbols ,and spaces.They are enclosed in single `(')` or double`(")` quotes.`(e.g , "Hello,world",'This is a string')`

