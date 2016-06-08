# Lists
In this chapter we discuss a very important data structure which is a python built-in data type "List". A list is a linear collection of data. It can store ANYTHING. Lists in python have dynamic size ie. their size is same as the number of contents in the list. Since a list is an object, it has many methods which can be used to manipulate it. Lists are mutable ie. their contents can be changed. 

In this chapter, we discuss about all these features of a list and show the most common operations on a list. 

## List usage
Let us create a simple variable called sample_list and assign a empty list to it.
```
sample_list = []
```
Instead of creating an empty we could have created a list with some values
```
sample_list = [1,2,'hello']
```

A list can contain any python object, be it integer,string, user-defined object etc.

## Finding list length
The len function gives length of a list
```
len(sample_list)
```

## Accessing list elements
List elements can be accessed using index
```
sample_list[0]
```
We can also use negative indices just like wge saw for strings, to access list elements in reverse order.
```
sample_list[-1] #gives 'hello'
```
## Slicing lists
Lists also support slicing, just like strings
```
sample_list[0:2] #returns new list [1,2]
sample_list[::-1] #returns new reversed list ie. ['hello',2,1]
```
## Nesting lists
Lists can have anything inside, thus they can have other lists as members
```
sample_list = [[1,2,3],[2,3],1,2]
```
Now we can access the first element in the second nested list
```
sample_list[1][0] # gives 2
sample_list[1] # gives [2,3]
```
## Looping through a list
Since lists are iterables we can use the for loop syntax with 'in' keyword to loop through
```
for element in sample_list:
  print(element)
```
### Program to sum a list of numbers
```
sum = 0
numbers = [2,3,5,6]
for number in numbers:
  sum += number
print(sum)
```
Although this program works we can use the sum( ) function straightaway
```
numbers = [2,5,6,7]
print(sum(numbers))
```

## Appending new elements to a list
We can append new elements to a list using the append( ) method
```
sample_list = [3,4,6]
sample_list.append(20)
print(sample_list) #prints [3,4,6,20]
```
The append( ) method takes object as argument and inserts it at the end of the list

## Inserting elements into a list (at any position)
The insert( ) method which is present in all list objects can be used to insert an element anywhere in the list.
```
sample_list = [2,3,4]
sample_list.insert(1,'hello')
print(sample_list) #prints [2,'hello',3,4]
```
The insert method takes 2 arguments,
* index where element has to be inserted
* element to insert

## Deleting elements from a list
There are two ways in which we can delete elements from a list
1. Using remove( ) method: We can use the remove( ) method of the list object to locate and remove an element(first occurrence) from a list. eg. ```sample_list.remove(2)```
2. Using del: If we know the index of the element we can use del. Eg. ```del sample_list[1]```

There are many more methods in the list object. You can refer the documentation.

## List comprehension
It is quite common to have problems where we want to generate and return a new list based on some computation. List comprehensions help us do that in a much easier way. Let us see an example:
**Write a program which gives list of even numbers from a list of numbers**
Here is an implementation without using comprehensions
```
even_numbers = [] 
given_numbers = [2,3,4,5,6,7]
for number in given_numbers:
  if number % 2 == 0:
    even_numbers.append(number)
    
print(even_numbers)
```
Here is the same program using list comprehension.

```
even_numbers = [number for number in given_numbers if number % 2 == 0]
print(even_numbers)
```
List comprehension can be used if:
* A new list needs to generated
* Nesting level of for loops is less than or equal to 2
* Only one if statement needs to be evaluated

## Sorting list
If a list contains only numbers or strings we can use the sort( ) method of list object to sort the list.
```
sample_list = [3,6,1,2]
sample_list.sort()
print(sample_list) #prints [1,2,3,6]
```






 



