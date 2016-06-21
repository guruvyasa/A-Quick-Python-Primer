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
  print('in function, number1 = ',number1,'number2= ',number2)
  
changeNumber(number1,number2)

print('Outside function, number1 = ',number1,'number2 = ',number2)


```