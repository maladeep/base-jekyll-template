---
date: 2019-07-29
title: Python Print 
categories:
  - python
description: Your guide to effective use of Python You can use single quotes or double quotes, but they need to be used together.
type: Document
---
Printing has been always the first step to dive into new language's power.The print function in Python is a function that outputs to the console window whatever we say we want to print out.

If you learn how to print properly,trust me,  you will be very good at debugging. (HOW?: Wait for my future post)

> "Debugging" is the term given to the act of finding, removing, and fixing errors and mistakes within code.

## How to print

Try running this code to see an example:

```python

  print('Python is Awesome')

```

Output

```python

Python is Awesome

```


## Single quote and Double quotes
We can use single quotes or double quotes, but they need to be used together.


```python

  print("Python is Awesome")
  print('Python is Awesome')

```

Output:

```python

Python is Awesome
Python is Awesome


```



## Joining two String 

Concatenation just means the combination of things. We can use the "+" or the "," to join strings together.


If we use a ",", then we will have a space in between the strings we joined. 

If we use a "+", then the strings will be strung together with no space. 

> Use as per need.

```python

print('We are not allowed to do this:'+5)
		
```


Output:
```python

Traceback (most recent call last):
  File "main.py", line 2, in <module>
    print('cannot do this:'+5)
TypeError: can only concatenate str (not "int") to str
		
```


Instead lets do:

```python

print('We are  allowed to do this:' ,5)
		
```

output:

```python

		We are  allowed to do this: 5
    
```

Noted that in above there is a space in between ... this: and 5



### Time to  put some effort
Today, We learn about printing in Python which will definately help us in our python journey.

If any queries, feel free to email me.
