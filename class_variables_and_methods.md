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
