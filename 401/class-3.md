# Primitives, Objects, Try/Catch



## [Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)

Every primitive has an object associated with it as well. The object takes up mustch more memory than the primitive.  

**Primitive memory allocation**  
- boolean – 1 bit
- byte – 8 bits
- short, char – 16 bits
- int, float – 32 bits
- long, double – 64 bits  

**Object footprint**
- Boolean – 128 bits
- Byte – 128 bits
- Short, Character – 128 bits
- Integer, Float – 128 bits
- Long, Double – 192 bits

It's important to take things things into account when you consider what kind of platform you can expect your program to be running. Some omay require more efficiency 
with processing power/ memory allocation etc. .
 

## [Exceptions in Java (read the first three sections on the left: What is an Exception, The Catch or Specify Requirement, Catching and Handling Exceptions)](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

- Exception -  An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.  
Exceptions are handled as objects that the method creates when there is an error. The runtime then looks to find a way to handle that error through a list of other methods.  

**Valid Java programming language code must honor the Catch or Specify Requirement. This means that code that might throw certain exceptions must be enclosed by either of the following:**

- A try statement that catches the exception. The try must provide a handler for the exception, as described in Catching and Handling Exceptions.
- A method that specifies that it can throw the exception. The method must provide a throws clause that lists the exception, as described in Specifying the Exceptions Thrown by a Method.

**3 types of exceptions**
1. checked exception - These are exceptional conditions that a well-written application should anticipate and recover from.  
2. error - These are exceptional conditions that are external to the application, and that the application usually cannot anticipate or recover from. Errors are not subject to the Catch or Specify Requirement. Errors are those exceptions indicated by Error and its subclasses. 
3. runtime exception - These are exceptional conditions that are internal to the application, and that the application usually cannot anticipate or recover from. These usually indicate programming bugs, such as logic errors or improper use of an API.

## [Using Scanner to read in a file in Java](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)

Objects of type [Scanner](https://docs.oracle.com/javase/8/docs/api/java/util/Scanner.html) are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.  
White spaces are used to seperate tokens which can then be checked for values or conditionals.  

