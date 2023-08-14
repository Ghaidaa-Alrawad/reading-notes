# Java OO

## Difference between an object and a class:

An object embodies a specific occurrence of a class, bundling both data (state) and functions (behaviors) relevant to that data. Visualize an object as a tangible entity with which interactions occur.

Conversely, a class serves as a foundational plan or model to generate objects. It establishes the framework, attributes, and actions that objects of that class will possess. In simpler words, a class is the concept or blueprint, while an object is its concrete manifestation.

## Two types of state that a Student object might have:

- Full Name: This could be stored as a string and hold the student's complete name.
- Age: Represented by an integer, it could store the student's age in years.

## Two types of behaviours that a student object might have:

- Study: This action involves methods that simulate studying, like "studySubject(subject)" or "takeNotes()". These methods mimic a student's learning process.

- Submit Assignment: This behavior might utilize a method such as "submitAssignment(assignment)" to simulate a student handing in their assignments.

---

# Java Classes

## Explaining the significance of a constructor for a class:

A constructor is a special method within a class that is automatically called when an object of that class is created. It initializes the object's state and sets up its initial values.

The constructor allows you to provide values for the fields of the object when you create it. This is essential for ensuring that the object starts in a valid state and is ready to be used without any uninitialized or undefined attributes.

Constructors play a crucial role in object-oriented programming by enabling proper object initialization and reducing the chance of errors due to uninitialized variables.

## Write the declaration statement for a class named “Student” :

`public class Student {`
`}`

---

# Binary, Decimal and Hexadecimal Numbers

## Value of the binary number 1101:

The binary number 1101 represents the decimal value of 13. To convert binary to decimal, you can use the powers of 2. Each digit in the binary number represents a power of 2, starting from the rightmost digit being 2^0, the next being 2^1, then 2^2, and so on.

So, in this case:

`(1 * 2^3 )+ (1 * 2^2) + (0 * 2^1) + (1 * 2^0) = 8 + 4 + 0 + 1 = 13`

## Number 52 in binary and hexadecimal:
Binary: To convert the decimal number 52 to binary, you can repeatedly divide the number by 2 and keep track of the remainders. 
Here's the breakdown:

`52 ÷ 2 = 26 remainder 0`
`26 ÷ 2 = 13 remainder 1`
`13 ÷ 2 = 6 remainder 1`
`6 ÷ 2 = 3 remainder 0`
`3 ÷ 2 = 1 remainder 1`
`1 ÷ 2 = 0 remainder 1`

Hexadecimal: To convert the decimal number 52 to hexadecimal, divide the number by 16 and keep track of the remainders.

Here's the breakdown:

`
52 ÷ 16 = 3 remainder 4 (4 is represented as "4" in hexadecimal)
3 ÷ 16 = 0 remainder 3 (3 is represented '3' in the hexadecimal)
`

`52 ÷ 16 = 3 remainder 4 (4 is represented as "4" in hexadecimal)`
`3 ÷ 16 = 0 remainder 3 (3 is represented '3' in the hexadecimal)`

---

## Things I want to know more about:

I want to learn more about advanced Java programming, in-depth object-oriented concepts, and exploring practical applications of different number systems