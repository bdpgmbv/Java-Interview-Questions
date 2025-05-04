1. Abstract

* Abstract class - you cannot create its objects directly
* Abstract method - has no body and must be overridden by child classes
* Notes: if a class has even 1 abstract method -> The class must be abstract
* Used when you want to force child classes to write certain methods


2. Final

* final variable - lock the variable (cant change it)
* final method - lock the method (cant override it) - java's Object.getClass()
* final class - lock the class (cant inherit it) - java's string class


3. Static

* static variable - Shared by all objects - changed it once, it updates for all objects
* static method - can be called without objects - can only call other static methods - can only access static variables - cannot use this or super keywords
* static blocks - runs when the class loads (e.g., loading config files)
* static nested class - cant be accessed without outer class object

* static members are stored in method area of the JVM memory

4. Access Specifiers
* public - No restriction - global access
* protected - Package + subclasses access (same package, diff package)
* default - package only access
* private - class only access 
