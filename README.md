4. What do you understand by Java Virtual Machine (JVM)?

* Is the engine to run Java program
* Converts bytecode into machine code and executes it.
* Makes java platform independent - Write once, run anywhere.

5. What is the difference between JDK, JRE, and JVM?

* JVM
  * Engine that runs the Java program
  * Converts (.class) bytecode into machine code and executes it. 
  * Manages memory (Heap, Stack, Garbage Collection)
  * Provides security by verifying bytecode.
  * !!!! JVM alone is not enough to run or develop java program !!!!
* JRE
  * Provides the minimum environment to run java program
  * Includes: JVM (to execute bytecode) + libraries (for core java classes)
  * Used by: end users who only need to run java apps (not 
