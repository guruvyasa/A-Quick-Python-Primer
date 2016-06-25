# Operator Overloading

Python also supports operator overloading. For example, suppose we have a list of students and we want to be able to use the + and - operators to add and subtract students. Why? Well, our definition of adding students is that we add only the marks. So,
```
class Student:
  def __init__(self,marks):
    self.marks = marks
```
