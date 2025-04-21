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
  * Used by: end users who only need to run java apps (not develop them)
  * !!!! JRE = JVM + Libraries (to run Java apps, but no compiler) !!!!
* JDK
  * Provides tools to develop, compile, and run Java Programs.
  * Includes: JRE (so you can run java programs) + Compiler (converts .java -> .class) + debugger, javadoc, jar, etc. (development tools).
  * !!!! JDK = JRE + Development tools (Compiler, Debugger, etc.,) !!!!
 
6. How many types of memory areas are allocated by the JVM?

* Method Area (Class Area):
   * Purpose: Stores class level data (like static variables, constructors, method data, bytecode, constant pool)
   * Shared: Yes (Shared across all threads)
* Heap Area
   * Purpose: Stores all objects and arrays.
   * Shared: Yes (Shared across all threads)
   * Managed by: Garbage Collector (GC)
* Stack Area
   * Purpose: Stores method calls, local variables, and partial results.
   * Shared: No (each thread has its own stack)
* Program Counter(PC) Register
   * Purpose: Keeps track of current instruction being executed in a thread.
   * Shared: No (each thread has its own PC register)
   * Note: If the method is native, PC register is undefined.
* Native method stack
   * Purpose: Stored native method calls (non-java code, like C/C++)
   * Shared: No (Each thread has its own native method stack)
 
7. What is JIT compiler ?
* Just In Time compiler is a key part of the JVM that makes Java programs run faster by converting freuently executed bytecode into optimzed machine code at runtime.

8. What is the Platform ?
* A platform refers to the combination of hardware and software on which programs run.
* In the context of java, the platform includes the operating system and the Java Virtual Machine.
