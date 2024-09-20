# OOP Interview Questions for First-Year Students

## 1. What is Object-Oriented Programming?

**Answer:** Object-Oriented Programming (OOP) is a programming paradigm that organizes code into objects, which are instances of classes. It focuses on the concept of objects that contain data and code. OOP is based on several principles that aim to increase flexibility and reusability in programming.

## 2. What are the four main principles of OOP?

**Answer:** The four main principles of OOP are:

1. Encapsulation
2. Inheritance
3. Polymorphism
4. Abstraction

## 3. Explain what a class is in OOP.

**Answer:** A class is a blueprint or template for creating objects. It defines the attributes (data) and methods (functions) that the objects of that class will have. Classes serve as a structure for bundling data and functionality together.

## 4. What is an object in OOP?

**Answer:** An object is an instance of a class. It is a concrete entity based on a class, and represents a specific instance of that class in memory. Objects have states (attributes) and behaviors (methods) as defined by their class.

## 5. What is encapsulation?

**Answer:** Encapsulation is the bundling of data and the methods that operate on that data within a single unit (like a class). It restricts direct access to some of an object's components, which is a means of preventing accidental interference and misuse of the methods and data.

## 6. What is inheritance in OOP?

**Answer:** Inheritance is a mechanism where a new class is derived from an existing class. The new class (subclass or derived class) inherits attributes and behaviors from the existing class (superclass or base class). This promotes code reusability and establishes a relationship between the parent and child classes.

## 7. Explain polymorphism with a simple example.

**Answer:** Polymorphism allows objects of different classes to be treated as objects of a common base class. A simple example is:

```python
class Animal:
    def speak(self):
        pass

class Dog(Animal):
    def speak(self):
        return "Woof!"

class Cat(Animal):
    def speak(self):
        return "Meow!"

def animal_sound(animal):
    print(animal.speak())

dog = Dog()
cat = Cat()

animal_sound(dog)  # Output: Woof!
animal_sound(cat)  # Output: Meow!
```

In this example, both `Dog` and `Cat` classes override the `speak` method. The `animal_sound` function can work with any `Animal` object, demonstrating polymorphism.

## 8. What is abstraction in OOP?

**Answer:** Abstraction is the process of hiding the complex implementation details and showing only the necessary features of an object. It helps in reducing programming complexity and effort. In OOP, abstraction can be achieved through abstract classes and interfaces.

## 9. What is the difference between a class and an object?

**Answer:** A class is a blueprint or template for creating objects. It defines the structure and behavior that the objects of that class will have. An object, on the other hand, is an instance of a class. It's a concrete entity based on the class, with actual values for its attributes and the ability to perform the methods defined in the class.

## 10. What is a constructor in OOP?

**Answer:** A constructor is a special method in a class that is automatically called when an object of that class is created. It is used to initialize the object's attributes. Constructors typically have the same name as the class and don't have a return type.
