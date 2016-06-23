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
Now we can start creating new students with different names and ages as;

```
student1 = Student('sathvik',22)
student2 = Student('chandan',2)
print("Student1 data ",student1.age,student1.name)
print("Student2 data ",student2.age,student2.name);
```
Every method in a class is passed a reference to the instance by default, and thus we need to have a parameter to hold it. We have used 'self' in our example to hold the reference to the current instance.

The \_\_init\_\_  method behaves like a constructor of the Student class, which takes the name and age, and creates a new student object with the given name and age.                                                                                                                                                                                                                                                                                                                                                                            