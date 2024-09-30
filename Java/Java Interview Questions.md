# Java Interview Questions

## Table of Contents
1. [What is Java?](#what-is-java)
2. [What are the main features of Java?](#what-are-the-main-features-of-java)
3. [What is the Java Virtual Machine (JVM)?](#what-is-the-java-virtual-machine-jvm)
4. [What is the difference between JDK, JRE, and JVM?](#what-is-the-difference-between-jdk-jre-and-jvm)
5. [What are the basic data types in Java?](#what-are-the-basic-data-types-in-java)
6. [What is a class in Java?](#what-is-a-class-in-java)
7. [What is an object in Java?](#what-is-an-object-in-java)
8. [What is inheritance in Java?](#what-is-inheritance-in-java)
9. [What is polymorphism in Java?](#what-is-polymorphism-in-java)
10. [What is encapsulation in Java?](#what-is-encapsulation-in-java)
11. [What are access modifiers in Java?](#what-are-access-modifiers-in-java)
12. [What is an interface in Java?](#what-is-an-interface-in-java)
13. [What is an abstract class in Java?](#what-is-an-abstract-class-in-java)
14. [What is the difference between an interface and an abstract class?](#what-is-the-difference-between-an-interface-and-an-abstract-class)
15. [What is method overloading?](#what-is-method-overloading)
16. [What is method overriding?](#what-is-method-overriding)
17. [What is the final keyword in Java?](#what-is-the-final-keyword-in-java)
18. [What is exception handling in Java?](#what-is-exception-handling-in-java)
19. [What are checked and unchecked exceptions?](#what-are-checked-and-unchecked-exceptions)
20. [What is a collection in Java?](#what-is-a-collection-in-java)
21. [What is the difference between ArrayList and LinkedList?](#what-is-the-difference-between-arraylist-and-linkedlist)
22. [What is a HashMap in Java?](#what-is-a-hashmap-in-java)
23. [What is the difference between == and equals() in Java?](#what-is-the-difference-between--and-equals-in-java)
24. [What is a String in Java?](#what-is-a-string-in-java)
25. [What is the StringBuilder class in Java?](#what-is-the-stringbuilder-class-in-java)
26. [What is the purpose of the this keyword in Java?](#what-is-the-purpose-of-the-this-keyword-in-java)
27. [What is a constructor in Java?](#what-is-a-constructor-in-java)
28. [What is a static method in Java?](#what-is-a-static-method-in-java)
29. [What is the significance of the main method in Java?](#what-is-the-significance-of-the-main-method-in-java)
30. [What are lambda expressions in Java?](#what-are-lambda-expressions-in-java)
31. [What is a functional interface in Java?](#what-is-a-functional-interface-in-java)
32. [What are Java Annotations?](#what-are-java-annotations)
33. [What is the Java Memory Model?](#what-is-the-java-memory-model)
34. [What is multithreading in Java?](#what-is-multithreading-in-java)
35. [What is synchronization in Java?](#what-is-synchronization-in-java)
36. [What are Java Streams?](#what-are-java-streams)
37. [What is the difference between ArrayList and Vector?](#what-is-the-difference-between-arraylist-and-vector)
38. [What is the volatile keyword in Java?](#what-is-the-volatile-keyword-in-java)
39. [What is the significance of the default keyword in interfaces?](#what-is-the-significance-of-the-default-keyword-in-interfaces)
40. [What are try-with-resources in Java?](#what-are-try-with-resources-in-java)

---

## What is Java?
<details>
<summary>Answer</summary>
Java is a high-level, object-oriented programming language designed for portability, performance, and security. It follows the principle of "Write Once, Run Anywhere" (WORA), meaning that Java code can run on any platform that has a Java Virtual Machine (JVM).
</details>

## What are the main features of Java?
<details>
<summary>Answer</summary>
- **Object-Oriented**: Java follows the principles of OOP, which includes encapsulation, inheritance, and polymorphism.
- **Platform-Independent**: Java code is compiled into bytecode that can be executed on any device with a JVM.
- **Automatic Memory Management**: Java uses a garbage collector to manage memory and reclaim unused objects.
- **Multithreaded**: Java supports multithreading, allowing concurrent execution of tasks.
- **Rich Standard Library**: Java provides a comprehensive set of APIs for various functionalities.
</details>

## What is the Java Virtual Machine (JVM)?
<details>
<summary>Answer</summary>
The Java Virtual Machine (JVM) is an abstract computing machine that enables a computer to run Java programs. It converts Java bytecode into machine code, allowing Java applications to be executed on any platform that has a JVM.
</details>

## What is the difference between JDK, JRE, and JVM?
<details>
<summary>Answer</summary>
- **JDK (Java Development Kit)**: A software development kit that provides tools for developing Java applications, including the JRE, compiler, and other tools.
- **JRE (Java Runtime Environment)**: A package that includes the JVM and libraries necessary to run Java applications but does not include development tools.
- **JVM (Java Virtual Machine)**: The component responsible for executing Java bytecode.
</details>

## What are the basic data types in Java?
<details>
<summary>Answer</summary>
Java has eight primitive data types:
- **byte**: 8-bit signed integer
- **short**: 16-bit signed integer
- **int**: 32-bit signed integer
- **long**: 64-bit signed integer
- **float**: 32-bit floating-point
- **double**: 64-bit floating-point
- **char**: 16-bit Unicode character
- **boolean**: Represents true or false values.
</details>

## What is a class in Java?
<details>
<summary>Answer</summary>
A class in Java is a blueprint for creating objects. It defines the properties (attributes) and behaviors (methods) that the objects created from the class can have. Classes are fundamental to Java’s object-oriented programming paradigm.
</details>

## What is an object in Java?
<details>
<summary>Answer</summary>
An object is an instance of a class. It represents a specific implementation of the class, encapsulating its state (attributes) and behavior (methods). Objects are created using the new keyword.
</details>

## What is inheritance in Java?
<details>
<summary>Answer</summary>
Inheritance is a mechanism in Java that allows one class to inherit properties and behaviors from another class. It promotes code reusability and establishes a relationship between classes. In Java, a class can extend another class using the extends keyword.
</details>

## What is polymorphism in Java?
<details>
<summary>Answer</summary>
Polymorphism is the ability of a single function or method to operate in different ways based on the object that invokes it. In Java, polymorphism is achieved through method overloading (compile-time) and method overriding (runtime).
</details>

## What is encapsulation in Java?
<details>
<summary>Answer</summary>
Encapsulation is the practice of wrapping data (attributes) and methods (functions) that operate on that data into a single unit, or class. It restricts direct access to some of the object's components and can prevent the accidental modification of data. Access modifiers (private, protected, public) are used to achieve encapsulation.
</details>

## What are access modifiers in Java?
<details>
<summary>Answer</summary>
Access modifiers define the visibility of classes, methods, and variables. Java has four access modifiers:
- **private**: Accessible only within the same class.
- **protected**: Accessible within the same package and by subclasses.
- **public**: Accessible from any other class.
- **default (no modifier)**: Accessible only within the same package.
</details>

## What is an interface in Java?
<details>
<summary>Answer</summary>
An interface is a reference type in Java that defines a contract for classes to implement. It can contain abstract methods (without a body) and constants. A class can implement multiple interfaces, supporting multiple inheritance.
</details>

## What is an abstract class in Java?
<details>
<summary>Answer</summary>
An abstract class is a class that cannot be instantiated and may contain abstract methods (methods without an implementation) as well as concrete methods (with implementation). Abstract classes are used to provide a base for subclasses to extend and implement the abstract methods.
</details>

## What is the difference between an interface and an abstract class?
<details>
<summary>Answer</summary>
- An interface can only contain abstract methods and constants, while an abstract class can contain both abstract and concrete methods.
- A class can implement multiple interfaces but can extend only one abstract class.
- Interfaces represent a contract, while abstract classes provide a common base for related classes.
</details>

## What is method overloading?
<details>
<summary>Answer</summary>
Method overloading occurs when multiple methods in the same class have the same name but different parameter lists (different types, number, or order of parameters). It allows methods to perform similar functions with different inputs.
</details>

## What is method overriding?
<details>
<summary>Answer</summary>
Method overriding occurs when a subclass provides a specific implementation of a method that is already defined in its superclass. The overridden method in the subclass must have the same name, return type, and parameters as the method in the superclass.
</details>

## What is the final keyword in Java?
<details>
<summary>Answer</summary>
The final keyword is used in Java to restrict the user from changing the value of a variable, overriding a method, or inheriting a class. When a variable is declared as final, it can be assigned only once. A final method cannot be overridden, and a final class cannot be subclassed.
</details>

## What is exception handling in Java?
<details>
<summary>Answer</summary>
Exception handling in Java is a mechanism to handle runtime errors, allowing the program to continue its execution instead of terminating abruptly. It involves using try-catch blocks to catch exceptions, and finally blocks can be used for cleanup operations.
</details>

## What are checked and unchecked exceptions?
<details>
<summary>Answer</summary>
- **Checked exceptions** are exceptions that are checked at compile-time. The programmer must handle these exceptions using try-catch blocks or declare them using the throws keyword. Examples include IOException and SQLException.
- **Unchecked exceptions** are exceptions that are not checked at compile-time, typically due to programming errors, and do not need to be declared. Examples include NullPointerException and ArrayIndexOutOfBoundsException.
</details>

## What is a collection in Java?
<details>
<summary>Answer</summary>
A collection in Java is a framework that provides an architecture to store and manipulate groups of objects. The Java Collections Framework includes interfaces like List, Set, and Map, and classes like ArrayList, HashSet, and HashMap, providing various data structures and algorithms for managing collections of objects.
</details>

## What is the difference between ArrayList and LinkedList?
<details>
<summary>Answer</summary>
- **ArrayList**: Uses a dynamic array to store elements, providing fast random access but slower insertions and deletions compared to LinkedList. It is generally preferred for storing and accessing data.
- **LinkedList**: Uses a doubly linked list to store elements, providing faster insertions and deletions but slower random access. It is preferred for scenarios where frequent insertions and deletions occur.
</details>

## What is a HashMap in Java?
<details>
<summary>Answer</summary>
A HashMap is a part of the Java Collections Framework that implements the Map interface. It stores key-value pairs, allowing for efficient retrieval based on keys. HashMap allows null values and one null key and does not maintain any order of its elements.
</details>

## What is the difference between == and equals() in Java?
<details>
<summary>Answer</summary>
- **==**: This operator compares the references of two objects, checking if they point to the same memory location.
- **equals()**: This method compares the content of two objects, determining if they are logically equivalent. It should be overridden in user-defined classes to provide meaningful comparison.
</details>

## What is a String in Java?
<details>
<summary>Answer</summary>
A String in Java is an immutable sequence of characters. Strings are created using string literals (e.g., `String str = "Hello";`) and provide methods for manipulation, such as substring, length, and concatenation. Because they are immutable, any modification results in a new String object.
</details>

## What is the StringBuilder class in Java?
<details>
<summary>Answer</summary>
StringBuilder is a mutable class in Java used for creating and manipulating strings. It allows modifications to strings without creating new objects, improving performance when multiple concatenations or modifications are needed. It provides methods like append, insert, and delete.
</details>

## What is the purpose of the this keyword in Java?
<details>
<summary>Answer</summary>
The `this` keyword in Java refers to the current object instance. It is used to differentiate between instance variables and parameters when they have the same name. It can also be used to call other constructors in the same class.
</details>

## What is a constructor in Java?
<details>
<summary>Answer</summary>
A constructor in Java is a special method that is called when an object is instantiated. It has the same name as the class and does not have a return type. Constructors are used to initialize the object's attributes.
</details>

## What is a static method in Java?
<details>
<summary>Answer</summary>
A static method in Java belongs to the class rather than any particular instance. It can be called without creating an object of the class. Static methods can access static variables and other static methods but cannot access instance variables directly.
</details>

## What is the significance of the main method in Java?
<details>
<summary>Answer</summary>
The `main` method in Java is the entry point of any standalone Java application. It must be declared as `public static void main(String[] args)`, and it is invoked by the Java Virtual Machine (JVM) to start the execution of the program.
</details>

## What are lambda expressions in Java?
<details>
<summary>Answer</summary>
Lambda expressions in Java are a feature introduced in Java 8 that allows the implementation of functional interfaces using a more concise syntax. They provide a way to pass behavior as a parameter and are used primarily for creating instances of functional interfaces.
</details>

## What is a functional interface in Java?
<details>
<summary>Answer</summary>
A functional interface is an interface that contains exactly one abstract method. It can have multiple default or static methods. Functional interfaces can be implemented using lambda expressions, enabling a functional programming style in Java. The `@FunctionalInterface` annotation can be used to indicate a functional interface.
</details>

## What are Java Annotations?
<details>
<summary>Answer</summary>
Java Annotations are metadata that provide information about the program but are not part of the program itself. Annotations can be used to provide instructions to the compiler, define custom annotations, or provide additional information at runtime. Common annotations include `@Override`, `@Deprecated`, and `@SuppressWarnings`.
</details>

## What is the Java Memory Model?
<details>
<summary>Answer</summary>
The Java Memory Model (JMM) defines how threads interact through memory and establishes rules for visibility, ordering, and atomicity of variables. It ensures that Java programs behave consistently in a multithreaded environment, providing guarantees about the visibility of shared variables between threads.
</details>

## What is multithreading in Java?
<details>
<summary>Answer</summary>
Multithreading in Java is a concurrent execution of two or more threads, allowing multiple tasks to be performed simultaneously. Java provides built-in support for multithreading through the `Thread` class and the `Runnable` interface, enabling the development of responsive applications.
</details>

## What is synchronization in Java?
<details>
<summary>Answer</summary>
Synchronization in Java is a mechanism that ensures that only one thread can access a resource at a time, preventing data inconsistency and race conditions. It can be achieved using synchronized methods or synchronized blocks, allowing safe access to shared resources in a multithreaded environment.
</details>

## What are Java Streams?
<details>
<summary>Answer</summary>
Java Streams is a feature introduced in Java 8 that provides a functional approach to processing sequences of elements, such as collections. It allows operations like filtering, mapping, and reducing to be performed in a declarative manner. Streams support both sequential and parallel execution.
</details>

## What is the difference between ArrayList and Vector?
<details>
<summary>Answer</summary>
- **ArrayList**: Not synchronized, making it more efficient for single-threaded applications. It allows for dynamic resizing and provides better performance for random access.
- **Vector**: Synchronized, making it thread-safe but slower compared to ArrayList. It also doubles its size when more space is needed.
</details>

## What is the volatile keyword in Java?
<details>
<summary>Answer</summary>
The `volatile` keyword in Java is used to indicate that a variable's value may be changed by different threads. Declaring a variable as volatile ensures that its latest value is always visible to all threads, preventing caching issues and ensuring proper visibility of shared data.
</details>

## What is the significance of the default keyword in interfaces?
<details>
<summary>Answer</summary>
The `default` keyword in interfaces, introduced in Java 8, allows the definition of default methods with a body. This enables the addition of new methods to interfaces without breaking existing implementations. Default methods provide a way to add functionality while maintaining backward compatibility.
</details>

## What are try-with-resources in Java?
<details>
<summary>Answer</summary>
Try-with-resources is a feature introduced in Java 7 that allows automatic management of resources, such as files or network connections. When a resource is declared within the parentheses of the try statement, it is automatically closed at the end of the statement, ensuring proper resource management and avoiding memory leaks.

```bash
try (BufferedReader br = new BufferedReader(new FileReader("file.txt"))) {
    // Use the resource
} catch (IOException e) {
    // Handle exception
}
```

</details>
