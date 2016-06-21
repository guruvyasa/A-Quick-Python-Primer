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



