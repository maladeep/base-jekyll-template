---
date: 2019-08-04
title: Multiple Value For Single Key in Dictionary 
categories:
  - python
description:  Have more than one value for a  key 
type: Document
---
If we want to have more than one value for a certain key, then we'll need to use a list or some other container for multiple values (another dict, a tuple, etc.). We can't do {"abc": 1, 2} as a dict is a key:value pair, with only one value per key. 

> However, we can do : Thanks to setdefault( ) function

First Lets create empty list

```python

x = {}

```
then let's using setdefault() append values to key:

```python

key = "mykey"
x.setdefault(key, [])
x[key].append(1)
x[key].append(5)
print(a)

```

Output

```python

{'mykey': [1, 5]}

```


### Reason?
We are able to attain this result because of setdefault( ) function.
as stated in W3school Python :  The setdefault( ) method returns the value of the item with the specified key. If the key does not exist, insert the key, with the specified value.

at next level we can combine setdefault( ) in this way also:


```python

  x.setdefault("mykey",[ ] ).append("quora")
  
```

Output:

```python

Python is Awesome
Python is Awesome


```



### Final code: 











```python

x = {}

key = "mykey"
x.setdefault(key, [])
x[key].append(1)
x[key].append(5)

x.setdefault("mykey",[ ] ).append("quora")
print(x)


		
```


Output:
```python

{'mykey': [1, 5, 'quora']}
		
```


[More on setdefault() ](https://docs.python.org/3/library/stdtypes.html)


[GitHub gist](https://gist.github.com/maladeep/9005ba128d7f1be954ad16d14c1ffb89)


### Time to  put some effort

Today, We learn about adding more than two one values in Python dictionary despite of dictionary  being  key:value pair, with only one value per key. 


If any queries, feel free to email me.
