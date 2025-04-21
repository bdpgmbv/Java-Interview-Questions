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

9. What are the main differences between the Java platform and other platforms ?
* Java is platform independent due to it "Write Once, Run anywhere" nature.
* Other platforms may require PLATFORM-SPECIFIC CODE AND COMPILATION FOR EACH TARGET ENVIRONMENT. 

10. What gives Java its 'write once and run anywhere' nature ?
* Java COMPILER CONVERTS the java program into class files (bytecode).
* Which is the intermediate state between SOURCE CODE AND MACHINE CODE.
* Bytecode is platform independent, and JVM executes this bytecode on any device with a compatible JVM.

11. What is a classloader?
* The classloader is a CORE PART OF THE JVM that loads classes into memory when they are needed.
* It ensures that the correct bytecode (.class files) is available for execution.

* The JVM uses 3 built-in class loaders in a hierarchy:
  * BootStrap ClassLoader
    * Parent: None (top-level)
    * Loads: Core java classes (java.lang, java.util etc.,)
    * Written in: Native code (not java)
  * Extension ClassLoader
    * Parent: BootStrap
    * Loads: Jars from jre/lib/ext (extension libraries)
  * Application ClassLoader
    * Parent: Extension
    * Loads: Classes from the classpath (your application code).

12. Is an empty .java file name a valid source file name ?
* An empty .java filename is not valid in Java.
* The filename must contain at least one character before the .java extension.
* Must match the public class name (if present) – If the file contains a public class, the filename must exactly match the class name (case-sensitive).

13. Is delete, next, main, exit or null keyword in java ?
* No, in Java, delete, next, main, exit, and null are not keywords.

14. If I do not provide any arguments on the command line, then what will the value stored in the String array passed into the main() method, empty or NULL?
* args is never null → The JVM INITIALIZES it as an EMPTY ARRAY if no arguments are provided.
* args.length == 0 → Indicates no arguments were passed.
* Safety: Prevents NullPointerException in the main method.

15. What if we write static public void instead of public static void?
* Java allows modifiers (public, static, final, etc.) in any order because they are independent of each other.
* The compiler only enforces that:
 * The return type (void, int, etc.) must appear right before the method name.
 * The method name + parameters follow correctly.
