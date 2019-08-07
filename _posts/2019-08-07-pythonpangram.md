---
date: 2019-08-07
title: Pangram in Python
categories:
  - python
description:  Checking pangram in Python 
type: Document
---
Pangram are words or sentences containing every letter of the alphabet at least once. Pangrams exist in practically every alphabet-based language whether it is english,spanish, nepali etc.

The most popular and oldest pangram is "The quick brown fox jumps over the lazy dog",which  has been used since at least the late 19th century.

Other Examples:

*  “Pack my box with five dozen liquor jugs.”

* “The jay, pig, fox, zebra and my wolves quack!”

* “Sympathizing would fix Quaker objectives.”

* "How vexingly quick daft zebras jump!"



##  Why we need them?

I still remember,when I first learned to type keyboard, my brother used to present the task of typing  "The quick brown fox jumps over the lazy dog", to ensure  that I am using  every key on the keyboard.

According to [Wikipedia ](https://en.wikipedia.org/wiki/Pangram), it was used in the days of the Telex/TWX  , to test if all letters could be broadcasted and received over a communication channel and  have been used to display typefaces, test equipment, and develop skills in handwriting, calligraphy, and keyboarding.




Now, Python code for checking Pangram.


```python

import string  
import sys
def ispangram(str1, alphabet=string.ascii_lowercase):
    alphaset = set(alphabet)
    return alphaset <= set(str1.lower())

print ( ispangram('The quick brown fox jumps over the lazy dog')) 

```

Output:

```
 True

```


Now replace the content in print statement i.e. (‘ The … dog’) with (‘Tora gives answer is not in dora’)

Output:

```
   False

```

## Inside code!


In above code, we imported two modules called 

* string :  Collection of string constant that gives pre-built  functionality of dealing with ASCII .Through this we are able              to use   .ascii_lowercase , .lower()
        

* sys :  Provides access to some objects used or maintained by the interpreter and to functions that interact strongly             with the interpreter.


and have used  build-in function called: set( )

Set( ) :  Recalling the  learning about sets and set theory at some point in our mathematical education, it is same like                  that (So, I assume you have good understanding about Set Theory) and It is similar to list ( ). list(s) generates a                 list of the characters in the string s. Similarly, set(s) generates a set of the characters in s and note that it will                  produce characters in unorders way.


>  Why didn't you use list( ) instead? 

Because in set( ), duplicate values are only represented in  once, i.e. by default we are presented with non duplicate values, which is what we need while checking pangram: 'every letter of the alphabet at least once.'

``` python

s = 'Mala'
print (list(s))
print (set(s))

```

Output:

```
['M', 'a', 'l', 'a']

{'M', 'a', 'l'}

```




### Time to  put some effort

Today, We learn about pangram and its usages and code for checking pangram through python.Now,try to create your own pangram and test it with code and  don't forget to share with me.

Happy Coding ^_^
