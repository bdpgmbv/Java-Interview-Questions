1. What is Java ?
* High level language, object oriented, platform independent, portable, secure, robust, high performance, multithreaded
* platform

2. What are the differences between C++ and Java ?

3. List the features of Java Programming language ?
* object oriented, high level, robust, secure, portable, high performance, multithreaded, platform independent, distributed

4. What do you understand by JVM ?
* Enables java to be platform independent
* provides a runtime environment to execute Java bytecode
* Functions - loads and verifies bytecode, Manages memory - Handles allocation (heap, stack) and garbage collection, Just in time compilation, 

5. What are the differences between JDK, JRE, and JVM?
* JVM - provides a runtime environment
* JRE - JVM + libraries
* JDK - JRE + development tools

6. How many types of memory areas are allocated by the JVM?
* stack - method calls, local variables 
* heap - objects, arrays (shared across threads)
* program counter register - current execution address 
* native method stack - Used for native method (written in C/C++)
* Method area - class metadata, static variables (shared across threads)

7. What is JIT compiler?
* JVM interprets bytecode line by line 
* JIT compiler identifies hotspots(frequently executed code)
* Compiles these hotspot into optimized native machine code

8. What is the platform?
* Combination of software and hardware on which programs run 

9. What are the main differences between the Java platform and other platforms?
* Java is write once run anywhere
* other programming languages may be need platform specific code/compilation

10. What gives Java its 'write once and run anywhere' nature?
* Java compiler converts Java code to class files(byte code)
* Intermediate language between Java code and the machine code is bytecode
* byte makes java platform independent, and can be executed in any platform with a compatible JVM

11. What is a classloader ?
* Loads classes into memory during runtime
* Bootstrap classloader: Loads all the jar files of Java Standard Edition
* Extension classloader: Loads all the jar files located in $JAVA_HOME/jre/lib/ext
* Application classloader: Loads all the jar files from the classpath

12. Is an empty .java file name a valid source file name?
* No, its not a valid file name - file name must match a class name.

13. Is delete, next, main, exit, or null keyword in Java?
* No delete, next, main, exit are not keywords and can be used as variables/method names 
* Null is a reserved literal

14. If I do not provide any arguments on the command line, then what will the value stored in the String array passed into the main() method, empty or NULL?
* args[] will be empty, not null
* JVM initializes args to an empty array to prevent nullpointerexception in case of argument checks

15. What if we write static public void instead of public static void ?
* access specifiers (public, private, protected)
* other specifiers (static, final, etc)
* Both of the above before the return type (void) is flexible

16. What is the default value of the local variables?
* In java, default values are never specified by the compiler

```
public class Main {
  public static void main(String[] args) {
    int x;
    System.out.println(x); // compilation error 
  }
}
```

17. What are the various access specifiers in Java?
* public - no restriction - global access
* protected - package + subclasses (same package, diff package)
* default - package only access
* private - class only access

18. What is the purpose of static methods and variables?
* create class level members - belongs to the class itself and not individual objects
* saves memory - as only one copy exists
* can be called without creating objects 

19. What are the advantages of packages in Java?
* Organize classes - like folders 
* Prevent name clashes - same class names allowed in different packages
* Hide sensitive code - only share whats needed
* reuse code - import and use classes easily

20. What is the output of the following Java program?
* System.out.println(10 + 20 + "Tpointtech");   // 30Tpointtech
* System.out.println("Tpointtech" + 10 + 20);  // Tpointtech1020

21. What is the output of the following Java program?
* System.out.println(10 * 20 + "Tpointtech");   // 200Tpointtech
* System.out.println("Tpointtech" + 10 * 20); // Tpointtech200

22. What is the output of the following Java program?
```java
for(int i=0; 0; i++) {  
  System.out.println("Hello Tpointtech");  
}  
```
* compilation error due to the non-boolean expression in the second part of the for loop

23. What is an object-oriented paradigm?
* writing programs by modelling them after real world objects
* Objects have - properties (what they are) and behaviour (what they do)

24. What is an object?
* modelled after real world objects
* have properties (variables) and behavious (methods)

25. What is the difference between an object-oriented programming language and an object-based programming language?
* OOP = objects + inheritance + polymorphism
* OBP = only objects

26. What will be the initial value of an object reference that is defined as an instance variable?
* null

27. What is the constructor?
* constructor in java is a special method that:
    * Automatically runs when an object is created (with new)
    * Initializes the object's properties (sets default values)
    * has the same name as class

28. How many types of constructors are used in Java?
* default constructor - created automatically by java if no constructor is defined. Intializes fields to default values (0, null, false) 
* parameterized constructor - takes arguments to intialize objects with custom values 

29. What is the purpose of a default constructor?
* created automatically by java if no constructor is defined.
* assigns default value to fields/properties (0, null, false)

30. Does the constructor return any value?
* No, not even void

31. Is the constructor inherited?
* No, constructors are not inherited in Java.
* Constructors are special methods tied to their own class.

32. Can you make a constructor final?
* No, you cannot declare a constructor as final in Java.
* Constructors are implicitly final (they cannot be overridden).

33. Can we overload the constructors?
* Yes! You can overload constructors in Java, just like method overloading.
* This means a class can have multiple constructors with different parameters.

34. What do you understand by copy constructor in Java?
* There is no copy constructor in Java.
* There are many ways to copy the values of one object into another in Java. They are:
    * By using a constructor
    * By assigning the values of one object to another
    * By using Object.clone() Method




