# Inheritance

Let us consider a simple example to illustrate inheritance. Suppose we have a Animal class defined as follows:
```
class Animal:
  def __init__(self,name,weight,age):
    self.name = name
    self.weight = weight
    self.age = age
  def set_name(self, new_name):
    self.name = new_name
```
If we create a new class Tiger which is a Animal as shown:
```
class Tiger(Animal): # Tiger is-a Animal
  pass
```
Here we have used inheritance to say that Tiger is a Animal. Now, we can access methods and variables from the Animal class. 
```
t = Tiger('sathvik',60,15)
print(t.age,t.name,t.weight) #60 sathvik 15
```
Although Tiger class does not define set_name method, age,name and weight attributes, it has these due to inheritance.

Python also supports multiple inheritance, here is an example,
Suppose we have a class called Vehicle, LandVehicle and WaterVehicle are its children. Suppose we want a new vehicle AmphibiousVehicle which is both a land and water vehicle. Here is how our class definitions may look like:
```
class Vehicle:
  def __init__(self,name,number):
    self.name = name
    self.number = number

class LandVehicle(Vehicle):
  def __init__(self,name,number):
    super().__init__(name,number)
    
class WaterVehicle(Vehicle):
  def __init__(self,name,number):
    super().__init__(name,number)

class AmphibiousVehicle(LandVehicle,WaterVehicle):
  def __init__(self,name,number):
    super().__init__(name,number)
    
    
am = AmphibiousVehicle('hoverBoat',2233) 
```

We will not talk about the potential flaws in this implementation, but nevertheless, this is how multiple inheritance is possible in python.
