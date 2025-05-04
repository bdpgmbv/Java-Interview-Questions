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

```
