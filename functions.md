# Functions
Everything is an object in python. So are functions. Functions help us(programmers) organize our code properly. We should remember that each function must have **single** responsibility.
Defining functions in python is easy as shown:
```
def addTwo(a,b): #definition
  return a+b
  
sum = addTwo(3,4) #function call
print(sum)
```
In the above example variables ```a``` and ```b``` are local variables, they are local to the function addTwo. Let us consider  
another example to illustrate this concept of local variables.

```
number1 = 10
number2 = 20
numbers = [[2,3],2,3,4]

def changeNumber(number1, number2):
  number1 = 30
  number2 = 40
  print('in function changeNumber, number1 = ',number1,'number2= ',number2)
  
def changeNumbers(numbers):
  numbers[1] = 222
  
  
changeNumber(number1,number2)

print('Outside function changeNumber, number1 = ',number1,'number2 = ',number2)

changeNumbers(numbers)
print('After executing changeNumbers ',numbers)

```

This program prints the following output:
```
in function changeNumber, number1 =  30 number2=  40
Outside function changeNumber, number1 =  10 number2 =  20
After executing changeNumbers  [[2, 3], 222, 3, 4]
```

If you observe the output here, values of number1 and number2 have remained the same after executing changeNumber. This shows variables number1 and number2 are local to the function changeNumber. They are passed by value ie. copies of those variables are passed.

On the other hand, numbers is a list and thus it gets passed **by reference**. So changes made inside ```changeNumbers``` function are visible outside too.


## Default arguments

Python allows us to assign default values to arguments of a function. Let us consider an example:
```

def addTwo(a=10,b=20):
  return a+b
  
print(addTwo()) # adds 10 and 20, prints 30
print(addTwo(20)) # adds 20 and 20, prints 40
print(addTwo(30,30) # adds 30 and 30, prints 60
```
As shown in the example, since both a and b have default values assigned, the call ```addTwo()``` just adds the default values of a and b. Similarly, the call ```addTwo(20)``` assigns the value 20 to a and b uses default value, ie 20.

Remember 2 rules when using default arguments:
* non-default argument cannot come after default argument. eg. ```def addTwo(a=10,b): #error
 ```
* Python does not support polymorphism the way c++ or java supports ie. we cant have 2 functions with the same name within the same scope. If given, the last function definition will override all others above it.


## Recursion

A function can call itself. Here is an example of such a recursive function to calculate the nth fibbonacci number.

```
def fib(n):
  if n == 1:
    return 0
  elif n == 2:
    return 1
  else:
    return fib(n-1) + fib(n-2)
```

In the function above we have made use of the fact that the nth fibonacci number is equal to sum of (n-1)th and (n-2)th fibonacci number








