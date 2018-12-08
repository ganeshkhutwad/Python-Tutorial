# Data Types

 - Integers (int):							Whole numbers: 10
 - Floating point (float):				Numbers with decimal point: 10.40
 - Strings (str):							Ordered sequence of characters: "hello"
 - Lists (list):								Ordered sequence of objects: [10, "hello", 200.3]
 - Dictionaries (dict):					Unordered Key: Value pairs: {"name": "Jessica"}
 - Tuples (tup):							Ordered immutalbe sequence of objects: (10, "hello", 10.2)
 - Sets (set):								Unordered collection of unique objects: {"a", "b"}
 - Booleans (bool):						Logical value indicating True or False

**Numbers**

 1. Integers which are whole numbers.
 2. Floating point numbers which are numbers with a decimal.

**Numbers FAQ**

**1. What's the difference between floating point and an integer?**

An integer has no decimals in it, a floating point number can display digits past the decimal point.  

**2. Why doesn't 0.1+0.2-0.3 equal 0.0 ?**

This has to do with floating point accuracy and computer's abilities to represent numbers in memory. For a full breakdown, check out: https://docs.python.org/2/tutorial/floatingpoint.html

**Variable Assignments**

 - Rules for variable names
	 - Names cannot start with a number.
	 - There can be no spaces in the name, use _ instead.
	 - Can't use any of these symbols
	 - :'",<>/?|\()!@#$%+&*~-+
	 - It's considered best practices (PEP8) that names are lowercase.
	 - Avoid using words that have special meaning in Python like "list" and "str"

**Dynamic Typing**

 - Python uses dynamic typing.
 - This means you can reassign variables to different data types.
 - This makes Python very flexible in assigning data types, this is different than other 	
    lanaguages that are **"Statically-Typed"**.
    
**Introduction to Strings**

 - Strings are sequences of characters, using the syntax of either single quotes or double quotes.
 - `"hello" or 'hi'`
 - Because strings are ordered sequences it means we can using indexing and slicing to grab sub-sections of the string.
 - Indexing notation uses [] notation after the string.
 - Indexing allows you to grab a single character from the string.

| character: | h | e | l | l | o |
|--|--|--|--|--|--|
| index: | 0 | 1 | 2 | 3 | 4 |
| reverse index: | 0 | -4 | -3 | -2 | -1 |

 - Slicing allows you to grab a subsection of multiple characters, a "slice" of the string.
 - `syntax: [start:stop:step]`
 - **start** is numerical index for the slice start
 - **stop** is the index you will go up to (but not include)
 - **step** is the size of the "jump" you take.

**Indexing and Slicing with Strings**

 - Indexing: grab a single character.
 - Slicing: grab a sub section of string.

**String properties and methods**

 - Addition:
 `x = 'Hello World'
 x = x + ' it is beautiful outside!'
 print(x)  // Hello World it is beautiful outside!`

 - Multiplication:
`letter = 'z'
print(letter * 10) // zzzzzzzzzz`

 - upper method:
 `x = 'Hello World'`
 `print(x.upper())`

 - lower method:
`x = 'Hello WORLD'`
`print(x.lower())`

 - split method:
`x = 'Hello World'`
`print(x.split())`

**Strings FAQ**

**1. Are strings mutable?**
Strings are not mutable! (meaning you can't use indexing to change individual elements of a string).

**2. How do I create comments in my code?**
You can use the hashtag # to create comments in your code.

**Print Formatting with Strings**
 - Often you will want to "inject" a variable into your string for printing. For example:
 `my_name = "Jose"
 print("Hello " + my_name)`
- There are multiple ways to format strings for printing variables in them.
- This is known as string interpolation.
- Let's explore two methods for this:
	- **.format()** method
	- **f-strings** (formatted strings literals)

**Formatting with the .format() method**
A good way to format objects into your strings for print statements is with the string .format() method. The syntax is:
`'String here {} then also {}'.format('something1','something2')`

Example:
`print('This is a string {}'.format('INSERTED'))`
`print('The {} {} {}'.format('fox', 'brown', 'quick'))`
`print('The {2} {1} {0}'.format('fox', 'brown', 'quick'))`
`print('The {q} {b} {f}'.format(f='fox', b='brown', q='quick'))`

**Float formatting follows "{value:width.precision f}"**
`result = 100/777`
`print("The result was {r:1.3f}".format(r=result))`

Here,
	r - actual value to print.
	width - spaces between string and value.
	precision - decimal point count.

**Formatting with the f-strings method**
`result = 100/777`
`print(f"The result was {result:1.3f}")`

**Print Formatting FAQS**

**1.) I imported print from the __future__ module, now print isn't working. What happened?**  

This is because once you import from the __future__ module in Python 2.7, a print statement will no longer work, and print must then use a print() function. Meaning that you must use

**print('Whatever you were going to print')**

or if you are using some formatting:

**print('This is a string with an {p}'.format(p='insert'****))**

The __future__ module allows you to use Python3 functionality in a Python2 environment, but some functionality is overwritten (such as the print statement, or classic division when you import division).

Since we are using Jupyter Notebooks, once you so the import, all cells will require the use if the print() function. You will have to restart Python or start a new notebook to regain the old functionality back.

**HERE IS AN AWESOME SOURCE FOR PRINT FORMATTING:**
[https://pyformat.info/](https://pyformat.info/)

**LISTS IN PYTHON**

 - Lists are ordered sequences that can hold a variety of object types.
 - They use [] brackets and commas to separate objects in the list.
	 - [1,2,3,4,5]
 - List support indexing and slicing. Lists can be nested and also have a variety of useful methods that can be called off of them.
 - Examples:
 `my_list = [1, 2, 3]`
 `my_list = ['Y', 100, 23.2]`
 `print(len(my_list))`
 `print(my_list[0])`
 `print(my_list[1:])`

**Concatenate a List**
`my_list = ["one", "two"]`
`another_list = ["three", "four"]`
`new_list = my_list + another_list`
`print(new_list) // ["one", "two", "three", "four"]`

**Lists FAQ**

**1. How do I index a nested list? For example if I want to grab 2 from [1,1,[1,2]]?**
You would just add another set of brackets for indexing the nested list, for example: my_list[2][1] . We'll discover later on more nested objects and you will be quizzed on them later!

**DICTIONARIES IN PYTHON**
- Dictionaries use curly braces and colons to signify the keys and their associated values.
`{"key1":"value1", "key2":"value2"}`
- So when to choose a list and when to choose a dictionary?

**Dictionaries:** Objects retrieved by key name. Unordered and can not be sorted.
**Lists:** Objects retrieved by location. Ordered sequence can be indexed or sliced.

**Dictionaries FAQ**

**1. Do dictionaries keep an order? How do I print the values of the dictionary in order?**
Dictionaries are mappings and do not retain order! If you do want the capabilities of a dictionary but you would like ordering as well, check out the  **ordereddict**  object lecture later on in the course!

**TUPLES WITH PYTHON**
