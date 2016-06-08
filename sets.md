# Sets
Sets are again important data structures which do not allow duplicate values. Let us look at an example:
```
sample_set = set([1,2,3,3,3,4]) #dont use { } here. it creates a dictionary not set!
print(sample_set) # prints {1,2,3,4}
```
In the example above we create a new set from a list ie. [1,2,3,3,3,4]. However, the new set only has 1,2,3,4. The duplicates have not been saved in the set. SETS DO NOT ALLOW DUPLICATES.

## Common set operations
Here are some example which show common set operations:
```
 a = set('abracadabra')
 b = set('alacazam')
 print(a)   # unique letters in a

 print(a - b)    # letters in a but not in b {'r', 'd', 'b'}
 print(a | b)   # letters in either a or b {'a', 'c', 'r', 'd', 'b', 'm', 'z', 'l'}
 print(a & b)    # letters in both a and b {'a', 'c'}
 print(a ^ b)   # letters in a or b but not both {'r', 'd', 'b', 'm', 'z', 'l'}
 
 ```
 ## Searching
 Similar to lists, tuples, strings the ```in``` keyword 
 ```
 print('a' in {'a','b','c'}) #prints True
 ```
 ## Set comprehension
 Similar to list comprehension we have set comprehension
 ```
 a = {x for x in 'abracadabra' if x not in 'abc'}
 print(a) # prints {'r','d'}
 ```
 
 
#Dictionaries
A dictionary is an unordered set of key: value pairs, with the requirement that the keys are unique (within one dictionary).

## Creating empty dictionary
A pair of empty flower braces creates an empty dictionary
```
empty_dict = { } 
```
## A simple dictionary example
Here is a simple example using dictionaries
```
sample_dict = {'name':'sathvik','estd':2015} # creates a dictionary
print(sample_dict['name']) # prints sathvik
print(sample_dict.get('estd')) # prints 2015
```
As shown we can get a value giving the key to the dictionary. We can either use [] or the get( ) method. Here are some more examples:
```
print(sample_dict.keys()) # prints ['name','estd']
print(sample_dict.values()) # prints ['sathvik',2015]
print('name' in sample_dict) # prints True
```

## Using dict( ) constructor
The ```dict( )``` constructor can be used to create a dictionary from sequences of values. Here are some examples:
```
my_dict1 = dict([('name', 'chandan'), ('age', 30)])
my_dict2 = dict(name='chandan',age=30)
```



