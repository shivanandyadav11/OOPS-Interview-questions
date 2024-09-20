# OOP Interview Questions for First-Year Students (Java)

## 1. What is Object-Oriented Programming?

**Answer:** Object-Oriented Programming (OOP) is a programming paradigm that organizes code into objects, which are instances of classes. It focuses on the concept of objects that contain data and code. OOP is based on several principles that aim to increase flexibility and reusability in programming.

## 2. What are the four main principles of OOP?

**Answer:** The four main principles of OOP are:

1. Encapsulation
2. Inheritance
3. Polymorphism
4. Abstraction

## 3. Explain what a class is in OOP.

**Answer:** A class is a blueprint or template for creating objects. It defines the attributes (data) and methods (functions) that the objects of that class will have. In Java, a class is defined using the `class` keyword. For example:

```java
public class Car {
    private String model;
    private int year;

    public void startEngine() {
        System.out.println("Engine started!");
    }
}
```

## 4. What is an object in OOP?

**Answer:** An object is an instance of a class. It is a concrete entity based on a class, and represents a specific instance of that class in memory. In Java, objects are created using the `new` keyword:

```java
Car myCar = new Car();
```

## 5. What is encapsulation?

**Answer:** Encapsulation is the bundling of data and the methods that operate on that data within a single unit (like a class). In Java, encapsulation is often achieved using private attributes and public getter and setter methods:

```java
public class BankAccount {
    private double balance;

    public double getBalance() {
        return balance;
    }

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }
}
```

## 6. What is inheritance in OOP?

**Answer:** Inheritance is a mechanism where a new class is derived from an existing class. In Java, inheritance is implemented using the `extends` keyword:

```java
public class Animal {
    public void eat() {
        System.out.println("This animal eats food.");
    }
}

public class Dog extends Animal {
    public void bark() {
        System.out.println("The dog barks.");
    }
}
```

## 7. Explain polymorphism with a simple example.

**Answer:** Polymorphism allows objects of different classes to be treated as objects of a common base class. In Java, this can be demonstrated through method overriding:

```java
public class Animal {
    public void makeSound() {
        System.out.println("The animal makes a sound");
    }
}

public class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("The dog barks");
    }
}

public class Cat extends Animal {
    @Override
    public void makeSound() {
        System.out.println("The cat meows");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal myDog = new Dog();
        Animal myCat = new Cat();
        
        myDog.makeSound();  // Output: The dog barks
        myCat.makeSound();  // Output: The cat meows
    }
}
```

## 8. What is abstraction in OOP?

**Answer:** Abstraction is the process of hiding complex implementation details and showing only the necessary features of an object. In Java, abstraction can be achieved through abstract classes and interfaces:

```java
public abstract class Shape {
    abstract double calculateArea();
}

public class Circle extends Shape {
    private double radius;

    public Circle(double radius) {
        this.radius = radius;
    }

    @Override
    double calculateArea() {
        return Math.PI * radius * radius;
    }
}
```

## 9. What is the difference between a class and an object?

**Answer:** A class is a blueprint or template for creating objects. An object is an instance of a class. In Java:

```java
// Class definition
public class Car {
    private String model;

    public Car(String model) {
        this.model = model;
    }
}

// Object creation
Car myCar = new Car("Tesla");
```

## 10. What is a constructor in OOP?

**Answer:** A constructor is a special method in a class that is automatically called when an object of that class is created. In Java, constructors have the same name as the class and don't have a return type:

```java
public class Student {
    private String name;
    private int age;

    // Constructor
    public Student(String name, int age) {
        this.name = name;
        this.age = age;
    }
}

// Usage
Student newStudent = new Student("Alice", 20);
```
