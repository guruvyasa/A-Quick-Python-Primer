# Strings
There is no char type in python. Only strings. Thus single quotes and double quotes both can be used for strings.
> \>>>my_name = 'chandan' #same as "chandan"

> \>>>type(my_name)

> class 'str'

By the way, pound or hash symbol ie # marks beginning of a comment.
The '+' operator when applied to strings concatenates them.
>\>>> my_name + ' '+ 'purohit'

>'chandan purohit'

Note that the original string did not change ie. the one in my_name. **Strings are immutable**. Thus although we can access characters of a string using indexes like my_name[1],my_name[2] we cannot modify its value as in :
>\>>>my_name[0] = 'b' 

>TypeError: 'str' object does not support item assignment

The '\*' operator can be used with strings if one of the operands is an int.
> \>>>2 * 'hello'

>'hellohello'

With the ```in``` operator, we can check whether a character/string appears in a string:
>\>>> 'ha' in 'chandan'

>True

Length of a string can be got from len() function
>\>>>len('aaa')
'ss
>3

Everything is an object in python. So are strings. We can easily know the methods available on strings through the interpreter console as:

>\>>>dir('ss') #'ss' is just a string, any object can be given to dir

Follow along

>\>>> s = 'chandan'

>\>>> s.upper()

>'CHANDAN'

>\>>>s.count('a') #gives count of number of occurences of 'a' in 'chandan'

You can get help for any of these functions by

>\>>>help(s.isalnum) #gives doc about isalnum method in object s


split() -> splits a string based on a delimiter if provided else split on space.
eg.

> \>>> s = "this is a sentence"

>\>>> words = s.split()

Here we get back list of words in the sentence.








