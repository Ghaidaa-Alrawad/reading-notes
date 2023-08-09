# Class 03 Reading

## Primitives vs. Objects:

### Explain the difference between an "int" and an "Integer" in Java:

The main difference between an "int" and an "Integer" in Java lies in their type nature. An "int" is a primitive data type that represents a simple integer value, while an "Integer" is a wrapper class that encapsulates an "int" value within an object. This distinction is important because primitive types are more memory-efficient and have faster access times, while objects like wrapper classes have more features and can be used in contexts that require objects (like collections and generics).

### What is the default value for ints? Integers?:

The default value for an "int" is 0. When you declare an "int" variable, it is automatically initialized with this default value if you don't explicitly assign a value to it. On the other hand, the default value for an "Integer" (wrapper class) is "null." Wrapper classes are reference types, and their default value is "null" until they are assigned an actual value.

### What is autoboxing? Unboxing?

Autoboxing: Autoboxing is the process of automatically converting a primitive data type to its corresponding wrapper class. In other words, when you assign a primitive value to a wrapper class variable, Java automatically converts the primitive value into an object of the wrapper class. For example:
`Autoboxing:`
`int primitiveInt = 5; Integer wrappedInt = primitiveInt;`

Unboxing: Unboxing is the opposite process of autoboxing. It involves automatically converting a wrapper class object back to its corresponding primitive value. When you retrieve the value from a wrapper class object, Java automatically extracts the primitive value. For example:
`Unboxing:`
`Integer wrappedInt = 10; int primitiveInt = wrappedInt;`

Autoboxing and unboxing make it easier to work with both primitive types and their corresponding wrapper classes, allowing for more flexible and convenient coding.

## Exceptions in Java:

### Three basic categories of exceptions: 

Checked Exceptions: These are exceptions that the compiler requires you to handle explicitly. They are subclasses of the Exception class (excluding RuntimeException and its subclasses). Examples include IOException, SQLException, and ClassNotFoundException.

Unchecked Exceptions (Runtime Exceptions): These are exceptions that the compiler does not require you to handle explicitly. They are subclasses of the RuntimeException class. Common examples include NullPointerException, ArrayIndexOutOfBoundsException, and ArithmeticException.

Errors: These are exceptional conditions that typically indicate serious problems that a reasonable application should not try to catch. Errors are often not recoverable and are usually caused by failures external to the application. Examples include OutOfMemoryError and StackOverflowError.

### What type of statement can you use to handle an exception?

To handle exceptions, you use a try-catch statement. The try block contains the code that might throw an exception, and the catch block(s) following it contain code to handle specific exceptions that may be thrown within the try block. The catch block catches and handles the exception, allowing the program to continue executing gracefully.
In this structure, if an exception of type ExceptionType1 is thrown within the try block, the corresponding catch block for ExceptionType1 will handle the exception. You can have multiple catch blocks to handle different types of exceptions that might be thrown.

## Using Scanner to read in a file in Java:

### Describe a situation where you think it would be useful to have a program that scans text:

One situation where it would be useful to have a program that scans text is when processing user input in a command-line interface. For instance, consider a command-line application where users need to provide various inputs, such as commands, options, and arguments. Using a program that scans text, you can break down the user's input into individual tokens and process them accordingly. This allows for more structured and efficient handling of user interactions.

Another scenario is when parsing data files with specific formats. For instance, if you have a CSV (Comma-Separated Values) file containing data entries, a program that scans text can read and parse each entry as separate tokens. This enables you to extract and process the data in a systematic manner.

### What is input from a Scanner broken down into?

Input from a Scanner is broken down into tokens. A token is a unit of data separated by a delimiter, which by default is whitespace (blanks, tabs, and line terminators). The Scanner object reads the input stream and identifies these tokens based on the specified delimiter. Each time the next() method is called on the Scanner object, it reads and returns the next token from the input. These tokens can be of various data types, such as strings or the Java language's primitive types (except for char), depending on how you choose to process and interpret the inp

## Things I want to know more about

1. More in-depth exploration of autoboxing and unboxing in Java.

2. Delving into memory management in Java, including the differences between primitive types and wrapper objects.