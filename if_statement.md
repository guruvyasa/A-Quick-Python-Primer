# if statement
Having become familiar with the indentation rule of python let us now look into the if statement.

The syntax for the simple if statement is:

```
if expression:
  statement1
  statement2
```
Python (obviously) has an else which can be associated with the if.
```
if expression:
  statement
else:
  statement
```
Let us write a simple program to check if a number is even or odd
```
number = 10
if number % 2 == 0:
  print('even')
else:
  print('odd')
  ```
Store this in a file called even_odd.py. If you are using IDLE you can run with the run button or if you want you can run from the command line by changing directory to the directory where your program is stored and typing ```python even_odd.py```

Python equivalent of else if is the elif statement.
```
number = 10
if number == 5:
  print('Number equal to 5')
elif number == 10:
  print('Number equal to 10')
else:
  print('Neither 5 or 10')
```

Nesting if statements is also quite easy, just notice the indentation.
```
number = 10
if number > 5:
  if number % 2 == 0:
    print('even and above 5')
  else:
    print('above 5 but not even')
else:
  print('less than 5')
  ```
  
 Although switch statement and ternary operator are not present in python, there is a cool short hand notation for the simple if statement. Look at the code below:
 ```
 message_string = None
 a = 10
 message_string = "hello" if a == 10 else "hi"
 ```
 In the code above, since value in a is 10, message_string will have the string "hello". 
