# Class 02 Reading

## Java Imports

### Analogy for Built-In Packages:

Imagine Java as a toolbox with different sections to hold various tools for building things. These sections are like built-in packages in Java, grouping tools (classes, interfaces) for specific tasks. For instance, "java.util" holds utility tools, "java.io" handles input/output, and "java.lang" contains essential tools

#### Examples of Built-In Packages:

-java.util: Toolbox with tools for collections, dates, randomness, and more

-java.io: Toolbox for handling files and streams

-java.net: Toolbox for networking tasks

-java.lang: Essential toolbox always available

#### Steps for Creating a New Package in IntelliJ:

-Open IntelliJ IDEA: Launch the IDE

-Create/Open Project: Begin or access a Java project

-Find Source Folder: Locate where the Java source code resides

-Right-Click Source Folder: Click with the right mouse button on the source folder

-New > Package: Go to "New" and select "Package."

-Enter Package Name: Type in the package name, following conventions

-Click OK: Confirm to create the package

-Add Classes/Files: Now you can create Java elements inside the new package

##### IntelliJ IDEA manages the package structure, keeping your project organized

---

## Different types of loops in Java

### Which loop types use a loop counter?

The loop types that use a loop counter are the "for" loop and the "do-while" loop. These loops involve incrementing or modifying a loop counter variable as part of their control mechanism

### Explain the difference between While and Do-While loops:

The main difference between the "while" loop and the "do-while" loop lies in when the loop condition is evaluated

-While Loop:
-In a "while" loop, the loop condition is checked before the execution of the loop's body. If the condition is false initially, the loop's body might never execute
-The loop continues executing as long as the condition remains true. If the condition becomes false at any point, the loop terminates

#### Example

while (condition) {
    // loop body
}

-Do-While Loop:
-In a "do-while" loop, the loop's body is executed at least once before the loop condition is checked. This guarantees that the loop body will execute at least once.
-After the initial execution of the loop body, the condition is checked. If the condition is true, the loop continues to execute; if it's false, the loop terminates.

#### Example

do {
    // loop body
} while (condition);

-In a "do-while" loop, the loop's body is executed at least once before the loop condition is checked. This guarantees that the loop body will execute at least once
-After the initial execution of the loop body, the condition is checked. If the condition is true, the loop continues to execute; if it's false, the loop terminates

#### the key distinction is that a "while" loop may not execute its body if the condition is initially false, while a "do-while" loop ensures that its body is executed at least once before evaluating the condition

---

## Java Arrays

### Describe 3 built-in methods for Arrays:

-binarySearch(Object[] a, Object key):

This method searches for a specified value (key) within a sorted array of objects (e.g., integers, doubles) using the binary search algorithm.
It returns the index of the search key if it's found in the array. If not found, it returns a negative value that indicates the insertion point where the key would be inserted to maintain the sorted order.
equals(long[] a, long[] a2):

This method determines whether two specified arrays of longs are equal to each other.
Arrays are considered equal if they have the same length and corresponding elements at the same indices are equal.
Similar methods are available for other primitive data types as well (e.g., equals(int[] a, int[] a2)).
fill(int[] a, int val):

This method assigns a specified integer value (val) to every element in the given array of integers (a).
It's a quick way to set all elements of the array to the same value, essentially "filling" the array with that value.
Similar methods are provided for other primitive data types (e.g., fill(double[] a, double val)).
How is the size of an array determined in Java?

In Java, the size of an array is determined when the array is created, and it cannot be changed later. The size of an array refers to the number of elements it can hold. When you create an array, you specify its size explicitly. For example:


int[] numbers = new int[5]; // This array can hold 5 integers


In this example, the size of the numbers array is set to 5. You can't change the size of this array after creation. The size of the array is defined by the integer value specified within the square brackets when using the new keyword to create the array. This size indicates how many elements the array can store. Once an array is created, its size remains constant throughout its lifetime

---

## Things I want to know more about

-Advanced Array Manipulation

-Sorting and Searching Algorithms

-Memory Management