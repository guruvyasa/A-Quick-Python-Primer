# Tuples

Tuples are immutable data structures in python. Curly braces '(' and ')' are used for tuples. Once a tuple is created we cannot change its contents.
```
sample_tuple = (1,2,3)
sample_tuple[2] = 'Hello' #error
```

## Accessing elements
Tuple elements can be accessed just like list and string elements, using indices
```
sample_tuple = (11,12,14,15)
print(sample_tuple[2]) # prints 14
```

## Slicing 
Tuples also support slicing and just like in strings and lists, a new tuple is created.
```
sample_tuple = (33,44,55,66,77)
print(sample_tuple[:2]) #prints (33,44)
print(sample_tuple[1:5:2]) #prints (44,66)
```

## Counting number of occurrences
Tuple objects have a count( ) method which can be used to count the number of occurrences of an element.
```
sample_tuple = (1,1,3,3,5,5,5)
print(sample_tuple.count(5)) # prints 3

```
## Getting position of an element
Use index( ) method of tuple object to get the index of an element
```
sample_tuple = (2,3,4)
print(sample_tuple.index(4)) # prints 2
```
## Unpacking a tuple
Here is an example of unpacking a tuple

```
number_1, number_2 = (2,3)
print(number_1,number_2) #prints 2 3
```
If number of values in the tuple is more than number of variables, then we need to use a \*
```
numbers = (3,4,5,6,7)
first_number, *other_numbers = numbers
print(first_number,other_numbers) # prints 3 [4,5,6,7]
```

