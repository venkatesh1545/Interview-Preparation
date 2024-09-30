# Object-Oriented Programming (OOP) Interview Questions

## Table of Contents
1. [What is Object-Oriented Programming (OOP)?](#what-is-object-oriented-programming-oop)
2. [What are the main principles of OOP?](#what-are-the-main-principles-of-oop)
3. [What is a class in OOP?](#what-is-a-class-in-oop)
4. [What is an object in OOP?](#what-is-an-object-in-oop)
5. [What is encapsulation, and why is it important?](#what-is-encapsulation-and-why-is-it-important)
6. [What is inheritance in OOP?](#what-is-inheritance-in-oop)
7. [What is polymorphism in OOP?](#what-is-polymorphism-in-oop)
8. [What is abstraction in OOP?](#what-is-abstraction-in-oop)
9. [What is the difference between an abstract class and an interface?](#what-is-the-difference-between-an-abstract-class-and-an-interface)
10. [Can you explain method overloading with an example?](#can-you-explain-method-overloading-with-an-example)
11. [Can you explain method overriding with an example?](#can-you-explain-method-overriding-with-an-example)
12. [What is the super keyword in Java?](#what-is-the-super-keyword-in-java)
13. [What are access modifiers in OOP?](#what-are-access-modifiers-in-oop)
14. [What is a constructor in OOP?](#what-is-a-constructor-in-oop)
15. [What is the difference between a constructor and a method?](#what-is-the-difference-between-a-constructor-and-a-method)
16. [What is the purpose of the final keyword in OOP?](#what-is-the-purpose-of-the-final-keyword-in-oop)
17. [What is multiple inheritance, and how does Java handle it?](#what-is-multiple-inheritance-and-how-does-java-handle-it)
18. [What is a static method in OOP?](#what-is-a-static-method-in-oop)
19. [What is a static variable in OOP?](#what-is-a-static-variable-in-oop)
20. [What is a destructor in OOP?](#what-is-a-destructor-in-oop)
21. [What are design patterns in OOP?](#what-are-design-patterns-in-oop)
22. [What is the Singleton pattern?](#what-is-the-singleton-pattern)
23. [What is the Factory pattern?](#what-is-the-factory-pattern)
24. [What is the Observer pattern?](#what-is-the-observer-pattern)
25. [What is the Strategy pattern?](#what-is-the-strategy-pattern)
26. [What is a composition in OOP?](#what-is-a-composition-in-oop)
27. [What is aggregation in OOP?](#what-is-aggregation-in-oop)
28. [What is the difference between aggregation and composition?](#what-is-the-difference-between-aggregation-and-composition)
29. [What is the use of the instanceof operator in Java?](#what-is-the-use-of-the-instanceof-operator-in-java)
30. [What are lambda expressions, and how do they relate to OOP?](#what-are-lambda-expressions-and-how-do-they-relate-to-oop)

---

### What is Object-Oriented Programming (OOP)?
Object-Oriented Programming (OOP) is a programming paradigm based on the concept of "objects," which can contain data (attributes) and code (methods). OOP focuses on using objects to design applications and computer programs, promoting greater flexibility, reusability, and organization in code.

---

### What are the main principles of OOP?
The four main principles of OOP are:
- **Encapsulation**: The bundling of data and methods that operate on that data within a single unit, or class. It restricts direct access to some components, protecting object integrity.
- **Inheritance**: The mechanism by which one class can inherit properties and behaviors from another class, promoting code reuse.
- **Polymorphism**: The ability to present the same interface for different underlying data types. It can be achieved through method overloading (compile-time) and method overriding (runtime).
- **Abstraction**: The process of hiding complex implementation details and showing only the essential features of the object.

---

### What is a class in OOP?
A class is a blueprint or template for creating objects in OOP. It defines a set of attributes (properties) and methods (functions) that the objects created from the class will have. Classes promote code reusability and organization.

---

### What is an object in OOP?
An object is an instance of a class. It represents a specific implementation of the class and encapsulates its state (attributes) and behavior (methods). Objects interact with one another through their methods.

---

### What is encapsulation, and why is it important?
Encapsulation is the practice of bundling data (attributes) and methods (functions) that operate on that data within a single unit (class). It restricts access to certain components and prevents unauthorized modification, ensuring data integrity and promoting a clear separation between an object's interface and implementation.

---

### What is inheritance in OOP?
Inheritance is a mechanism that allows one class (subclass or derived class) to inherit properties and behaviors from another class (superclass or base class). It promotes code reuse and establishes a hierarchical relationship between classes.

---

### What is polymorphism in OOP?
Polymorphism allows objects to be treated as instances of their parent class rather than their actual class. It can be achieved through:
- **Method Overloading**: Multiple methods with the same name but different parameters within the same class.
- **Method Overriding**: A subclass provides a specific implementation for a method already defined in its superclass.

---

### What is abstraction in OOP?
Abstraction is the process of hiding the complex implementation details and exposing only the essential features of an object. It helps simplify interactions and reduces complexity by providing a clear interface for users.

---

### What is the difference between an abstract class and an interface?
- **Abstract Class**: Can contain both abstract methods (without an implementation) and concrete methods (with an implementation). A class can inherit from only one abstract class (single inheritance).
- **Interface**: Contains only abstract methods (Java 8 and later can have default and static methods). A class can implement multiple interfaces (multiple inheritance).

---

### Can you explain method overloading with an example?
Method overloading occurs when multiple methods in the same class have the same name but different parameter lists. For example:

```java
class MathOperations {
    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }
}
```
---

### Can you explain method overriding with an example?
**Answer:**
Method overriding occurs when a subclass provides a specific implementation for a method already defined in its superclass. For example:

```java
class Animal {
    void sound() {
        System.out.println("Animal makes a sound");
    }
}

class Dog extends Animal {
    void sound() {
        System.out.println("Dog barks");
    }
}
```

---
### What is the super keyword in Java?
**Answer:** The super keyword is used in Java to refer to the superclass (parent class) of the current object. It is used to access superclass methods and constructors, enabling subclasses to inherit behavior from their parents.

---

### What are access modifiers in OOP?
**Answer:** Access modifiers control the visibility of classes, methods, and variables. Common access modifiers include:

- ``private:`` Accessible only within the same class.

- ``protected:`` Accessible within the same package and by subclasses.

- ``public:`` Accessible from any other class.

- ``default (no modifier):`` Accessible only within the same package.
---
### What is a constructor in OOP?
**Answer:** A constructor is a special method used to initialize objects of a class. It has the same name as the class and does not have a return type. Constructors can be overloaded to create objects with different initial values.

---

### What is the difference between a constructor and a method?
**Answer:** 
- ``Constructor:`` Initializes a new object and has the same name as the class. It does not have a return type.
- ``Method:`` Defines the behavior of an object and can be called multiple times on an object. It has its own name and a return type.
---

### What is the purpose of the final keyword in OOP?
**Answer:** The final keyword is used to declare constants, prevent method overriding, and prevent inheritance. When applied to:

- ``Variables:`` It makes the variable immutable (its value cannot be changed).
- ``Methods:`` It prevents the method from being overridden in subclasses.
- ``Classes:`` It prevents the class from being subclassed.
---

### What is multiple inheritance, and how does Java handle it?
**Answer:** Multiple inheritance refers to a feature where a class can inherit from multiple classes. Java does not support multiple inheritance with classes to avoid ambiguity (the "Diamond Problem"). Instead, it allows multiple inheritance through interfaces, enabling a class to implement multiple interfaces.

---

### What is a static method in OOP?
A static method belongs to the class rather than any specific object instance. It can be called without creating an instance of the class and can only access static variables and other static methods directly.

---

### What is a static variable in OOP?
**Answer:** A static variable is shared among all instances of a class. It belongs to the class itself rather than any individual object. Static variables are used to store class-level data.

---

### What is a destructor in OOP?
**Answer:** A destructor is a special method used to perform cleanup operations before an object is destroyed. In languages like C++, it is called automatically when an object goes out of scope or is deleted. Java has garbage collection and does not have explicit destructors.

---

### What are design patterns in OOP?
**Answer:** Design patterns are reusable solutions to common software design problems. They represent best practices that can be applied in various situations to improve code organization, flexibility, and maintainability.

---

### What is the Singleton pattern?
**Answer:** The Singleton pattern ensures that a class has only one instance and provides a global point of access to that instance. This is useful for managing shared resources, such as configuration settings.

---

### What is the Factory pattern?
**Answer:** The Factory pattern provides an interface for creating objects without specifying the exact class of object that will be created. It allows subclasses to alter the type of objects that will be created.

---

### What is the Observer pattern?
**Answer:** The Observer pattern defines a one-to-many dependency between objects so that when one object (the subject) changes state, all its dependents (observers) are notified and updated automatically.

---

### What is the Strategy pattern?
**Answer:** The Strategy pattern enables selecting an algorithm's behavior at runtime. It defines a family of algorithms, encapsulates each one, and makes them interchangeable, allowing the algorithm to vary independently from clients.

---

### What is a composition in OOP?
**Answer:** Composition is a design principle where a class is composed of one or more objects from other classes, establishing a "has-a" relationship. This promotes code reuse and flexibility.

---

### What is aggregation in OOP?
**Answer:** Aggregation is a specialized form of association that represents a "whole-part" relationship where the part can exist independently of the whole. It implies a weaker relationship compared to composition.

---

### What is the difference between aggregation and composition?
**Answer:** The main difference is the strength of the relationship:

- ``Aggregation:`` Represents a "whole-part" relationship where the part can exist independently (e.g., a classroom can exist without a school).
- ``Composition:`` Represents a stronger relationship where the part cannot exist independently (e.g., a house cannot exist without rooms).

---

### What is the use of the instanceof operator in Java?
**Answer:** The instanceof operator is used to test whether an object is an instance of a specific class or an interface. It helps ensure type safety during runtime.

---

### What are lambda expressions, and how do they relate to OOP?
**Answer:** Lambda expressions are a feature introduced in Java 8 that allows you to express instances of functional interfaces (interfaces with a single abstract method) in a more concise and readable way. They are used to create anonymous functions and can simplify code, especially when working with collections and streams.

---