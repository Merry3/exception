# What is an Exception?

An exception (or exceptional event) is a problem that arises during the execution of a program. When an Exception occurs the normal flow of the program is disrupted and the program/Application terminates abnormally and an error message is displayed on the screen. which is not recommended, therefore, these exceptions  are to be handled. 

The Exception Handling in Java is one of the powerful mechanism to handle the runtime errors so that the normal flow of the application can be maintained.
An exception can occur for many different reasons. Following are some scenarios where an exception occurs.

•	Whenever a user provides invalid data.

•	The file requested to be accessed does not exist in the system.

•	When the Java Virtual Machine (JVM) runs out of memory.

•	Network drops in the middle of communication.

The parent class of all the exception classes is the java.lang.Exception class. we talk about the Exception class, it is a subclass of the built-in Throwable class.
 
There are some important methods available in the Throwable class which are as follows:

•	public String getMessage() – Provides information about the exception that has occurred through a message, which is initialized in the Throwable constructor.

•	public Throwable getCause() – Provides root cause of the exception as represented by a Throwable object.

•	public void printStackTrace() – Used to display the output of toString() along with the stack trace to System.err (error output stream).

•	public StackTraceElement [] getStackTrace() – Returns an array with each element present on the stack trace. The index 0 element will symbolize the top of the call stack, and the last element of array will identify the bottom of the call stack.

There are mainly two types of exceptions in Java as follows:

•	Checked exception

•	Unchecked exception

#Checked exceptions are also known as compile-time exceptions as these exceptions are checked by the compiler during the compilation process to confirm whether the exception is handled by the programmer or not. If not, then the system displays a compilation error. 
Examples of checked exceptions:-

•	SQLException is a checked exception that occurs while executing queries on a database for Structured Query Language syntax.

•	ClassNotFoundException is a checked exception that occurs when the required class is not found -- either due to a command-line error, a missing CLASS file or an issue with the classpath.

#Unchecked exceptions − An unchecked exception is an exception that occurs at the time of execution. These are also called as Runtime Exceptions. These include programming bugs, such as logic errors or improper use of an API. Runtime exceptions are ignored at the time of compilation.

Examples of unchecked exceptions:-

•	IllegalStateException is an unchecked exception that occurs when an environment's state does not match the operation being executed.

•	IllegalArgumentException is an unchecked exception that occurs when an incorrect argument is passed to a method.

•	NullPointerException is an unchecked exception that occurs when a user tries to access an object using a reference variable that is null or empty.

•	ArrayIndexOutofBound This type of exception occurs when you try to access an array with an invalid index value.

•	NumberFormatException This type of exception occurs when you pass a string to a method that cannot be converted to a number. 

•	ArithmeticException This type of exception occurs when you perform an incorrect arithmetic operation. For example, if you divide any number by zero, it will display such an exception.

#Errors − These are not exceptions at all, but problems that arise beyond the control of the user or the programmer. Errors are typically ignored in your code because you can rarely do anything about an error. For example, if a stack overflow occurs, an error will arise. They are also ignored at the time of compilation.

#Java try and catch

The try statement allows you to define a block of code to be tested for errors while it is being executed.

The catch statement allows you to define a block of code to be executed, if an error occurs in the try block.

The try and catch keywords come in pairs:

#Syntax

try {

  //  Block of code to try
  
}
catch(Exception e) {

  //  Block of code to handle errors
  
}


