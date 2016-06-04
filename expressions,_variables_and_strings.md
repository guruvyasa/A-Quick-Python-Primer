# Expressions, Variables and Strings
Before we start, you need to start a new python interpreter session. Python interpreter is a software which can intrepret and run python programs. It runs through your python program line-by-line executing each one at a time. Thus you can either open up an interactive interpreter session and try out python instructions one at a time or feed your entire python program as input to the interpreter. We will be working in the interactive interpreter in this chapter. 

### Starting interactive interpreter
#### Linux:
> $python3 [enter]
 
#### Windows:
* install python3 
* open IDLE ide and launch interpreter or in the command line enter python followed by enter key

Once the interpreter is running you will see a prompt like
> \>>>


**Note: It is better to use ipython console than the default python console as it provides many features including indentation out-of-the-box **

You can now start typing in any python command here:
Eg:
> \>>>1 + 2

> 3

> \>>>2 * 3

> 6

> \>>>2 - 3

> -1

Here we tested +,- and * operators for addition,subtraction and multiplication respectively. The interpreter echoes the output of the expression evaluated. Let us see the division operator now.

> 
> \>>>2 / 3

> 0.6666666666666666

> \>>>2 // 3

>0

There are two division operators in python 3, **/** for real division (gives actual quotient) and **//** gives the truncated result.

Python also has a power operator **\*\***
>\>>>2 \*\* 3

>8

**%** is the modulus operator
> \>>>3.5 % 2

>1.5

Python also has many built-in functions to perform common tasks like abs(),max(),min() etc.
>\>>> abs(-1)

>1

>\>>>max(1,2,3)

>3

Thus, integer(int),floating point(float) are amongst the basic data types in python. We can check type of any variable or constant like so.
>\>>>type(3.5)

>class 'float'

**Note: If you observe here everything is an object in python, including ints and floats**

### Variables
It is very easy to use variables in python. You dont need to worry about types. Python takes care of that for you. It is a dynamically typed language.
>\>>> a = 10;b=20

>\>>>print(a,b)

>10 20

Here we used the print() function to print the results on the screen.
In python variable names are just names, they can be names of anything. For example the value in variable a is now 10. We can change it to anything and python will not complain.

>\>>>type(a)

>class 'int'

>\>>>a = 2.5

>\>>>type(a)

>class 'float'

####Swapping the python way
Since python is extremely humane language and because variable names are indeed just names swapping values of two variables is just a one-liner!!
>\>>>a,b = 2.4,5

>\>>>a

>2.4

>\>>>b

>5

>\>>>b,a = a,b

>\>>>print(a,b)

>5 2.4

####Variable names
The characters making up a variable name can be lowercase and uppercase letters from the
alphabet (a through z and A through Z), the underscore character (_), and, except for the
first character, digits 0 through 9:


* myList and _list are OK, but 5list is not.
* list6 and l_2 are OK, but list-3 is not.
* mylist and myList are different variable names.

Even when a variable name is “legal” (i.e., follows the rules), it might not be a “good”
name. Here are some generally accepted conventions for designing good names:

* A name should be meaningful: Name price is better than name p.
* For a multiple-word name, use either the underscore as the delimiter (e.g., temp_varand interest_rate) or use camelCase capitalization (e.g., tempVar, TempVar,interestRate or InterestRate); pick one style and use it consistently throughout your program. 

* Shorter meaningful names are better than longer ones.

The below names are used as reserved keywords of the Python language. You cannot use them other than as Python commands.

```
False None True and as assert break class continue def
del elif else except finally for from global if import
in is lambda nonlocal not or pass raise return try while
with yield
```

























