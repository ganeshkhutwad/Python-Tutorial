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
    
