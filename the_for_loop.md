# The for loop
As mentioned the for loop in python is different. It is actually a foreach loop. Let us look at an example:
How do you print your name 10 times?
```
for i in range(10):
  print('chandan')
  
```
* the range( ) function is a utility function which can be used to generate a set of numbers within a range. Its syntax is range(start,stop,step)
* range(10) -> generates numbers between 0 and 10 (not including 10). This is NOT exactly what happens, but we can safely assume this way for now.
* range(1,10) -> 1,2,3,..,9
* range(1,10, 2) -> 1,3,5,7,9
*

In the loop example above the variable i takes on the values 0,1,2,..,9 on the 1st,2nd,3rd,...,10th iteration respectively.

We can nest for loops.
```
for i in range(10):
  for j in range(10):
    print(i,j)
```
We can easily print all characters of a string using a for loop
```
name = 'chandan'
for character in name:
  print(character)
```
This is possible because a string is an iterable object. We can loop through an object if it is iterable.
Python has a useful utility function call zip( ) to iterate through multiple iterables simultaneously. Here is an example to iterate through two strings.
```
for c1,c2 in zip('hello','hate'):
  print(c1,c2)
```
Here is the output of the above program
```
h h
e a
l t
l e
```
One thing to notice here is that zip considers the smallest length iterable for zipping through. Thus the for loop iterates only 4 times ie. length of 'hate'.
The for loop is generally preferred when the number for times the loop has to run is fixed.