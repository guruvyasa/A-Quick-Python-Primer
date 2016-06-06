# The for loop
As mentioned the for loop in python is different. It is actually a foreach loop. Let us look at an example:
How do you print your name 10 times?
```
for i in range(10):
  print('chandan')
  
```
* the range( ) function is a utility function which can be used to generate a set of numbers within a range. Its syntax is range(start,stop,step)
* range(10) -> generates numbers between 0 and 10 (not including 10)
* range(1,10) -> 1,2,3,..,9
* range(1,10, 2) -> 1,3,5,7,9

In the loop example above the variable i takes on the values 0,1,2,..,9 on the 1st,2nd,3rd,...,10th iteration respectively.
