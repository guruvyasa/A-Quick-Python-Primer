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






