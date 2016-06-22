# Classes and Objects

Creating a class in python is pretty simple. Here is an example which creates a class called Student.

```
class Student:
  pass
```
To create an instance of the class, just use the class as of it were a function, as shown.

```
student1 = Student()
```
Now we have a new object called student1 which is an instance of Student class. We can give this student a name and age,

```
student1.name = "sathvik"
student1.age = 22
```
However, the name and age attributes are present in only the student1 object, not in all objects created as students. Since every student has a name and age, we can make those attributes part of the class.

```
class Student:
  def __init__(self,name,age):
    self.name = name
    self.age = age
```
Now we can start creating new students with different names and ages as,

```
student1 = Student('sathvik',22)
student2 = Student('chandan',2S
```
                                                                                                                                                                                                                                                                                                                                                                                           