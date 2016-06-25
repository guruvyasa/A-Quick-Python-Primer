# Class Variables and Methods

Python also supports creation of class variables. Here is an example for the same

```
class Student:
  count = 0
  def __init__(self):
    Student.count += 1
    print(str(Student.count) + ' students created so far')
    
s1 = Student() //prints 1 students created so far
s2 = Student() //prints 2 students created so far
```
In this example, we have a Student class which contains an attribute called **count**. This is a class variable. We can access it through the class as ```Student.count```. We have incremented this count value in the \_\_init\_\_ function. 
Class variables are common to all objects. Thus, if a class variable is modified in a object all other objects will also see the modified value.

##Class methods

Class methods or static methods can be created using the @staticmethod decorator as shown in the following example:
```
class Student:
  count = 0
  def __init__(self):
    Student.count += 1
   
  @staticmethod
  def getStudentCount(self):
    print(Student.count)
  
s1 = Student() //prints 1 students created so far
s2 = Student() //prints 2 students created so far

Student.getStudentCount() //prints 2


