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


