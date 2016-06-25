# Operator Overloading

Python also supports operator overloading. For example, suppose we have a list of students and we want to be able to use the + and - operators to add and subtract students. Why? Well, our definition of adding students is that we add only the marks. So,
```
class Student:
  def __init__(self,marks):
    self.marks = marks
    
s1 = Student(20)
s2 = Student(30)
print(s1 + s2) #error, + operator does not support adding of Student objects
```
If we really want this, we need to overload the \_\_add\_\_ method in the Student class.Here is how to do it,
```
class Student:
  def __init__(self,marks):
    self.marks = marks
  def __add__(self,st):
    return self.marks + st.marks

s1 = Student(20)
s2 = Student(30)
print(s1 + s2) #prints 50
```

