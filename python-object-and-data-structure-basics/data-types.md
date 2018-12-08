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

 1. Slicing allows you to grab a subsection of multiple characters, a "slice" of the string.
 2. `syntax: [start:stop:step]`
 3. **start** is numerical index for the slice start
 4. **stop** is the index you will go up to (but not include)
 5. **step** is the size of the "jump" you take.

**Indexing and Slicing with Strings**

 6. Indexing: grab a single character.
 7. Slicing: grab a sub section of string.

**String properties and methods**

 1. Addition:
 `x = 'Hello World'
 x = x + ' it is beautiful outside!'
 print(x)  // Hello World it is beautiful outside!`

2. Multiplication:
`letter = 'z'
print(letter * 10) // zzzzzzzzzz`

3. upper method:
 `x = 'Hello World'`
 `print(x.upper())`

4. lower method:
`x = 'Hello WORLD'`
`print(x.lower())`

5. split method:
`x = 'Hello World'`
`print(x.split())`

**Strings FAQ**

**1. Are strings mutable?**
Strings are not mutable! (meaning you can't use indexing to change individual elements of a string).

**2. How do I create comments in my code?**
You can use the hashtag # to create comments in your code.

