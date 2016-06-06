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
The insert( ) 


 



