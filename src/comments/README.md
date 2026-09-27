# 💬 Java Comments — Beginner Practice

This section introduces **comments in Java** and explains how they are used to add notes, explanations, documentation, and temporarily disable code.

Comments are ignored by the compiler and are not executed as part of the program.

---

## 🎯 Learning Objectives

By completing this section, you will understand:

* What comments are
* Why comments are used
* Single-line comments
* Multi-line comments
* Documentation comments
* Commenting out code
* Comments placed after code
* When comments are useful
* Basic commenting practices

---

# 1. What Are Comments?

Comments are text written inside source code to provide information for developers.

Java does not execute comments as program instructions.

Example:

```java id="x3v6y8"
class Comments01 {
    public static void main(String[] args) {

        // This is a comment

        System.out.println("Hello World!");
    }
}
```

The comment is ignored when the program runs.

---

# 2. Single-Line Comments

A single-line comment starts with:

```java id="w3x2qz"
// 
```

Everything after `//` on that line is treated as a comment.

### Example

```java id="0cgf4u"
class SingleLineComment {
    public static void main(String[] args) {

        // This prints Hello World!
        System.out.println("Hello World!");

    }
}
```

The comment does not affect the output.

---

## Multiple Single-Line Comments

```java id="c9z0qk"
class SingleLineComments {
    public static void main(String[] args) {

        // This is my note
        // Java is a programming language
        // This code prints a message

        System.out.println("Hello Java!");

    }
}
```

Each line starts with `//`.

---

# 3. Multi-Line Comments

Multi-line comments start with:

```java id="b2y8jh"
/*
```

and end with:

```java id="0o4xkw"
*/
```

Everything between them is treated as a comment.

### Example

```java id="3h6m1u"
class MultiLineComment {
    public static void main(String[] args) {

        /*
         This is my book
         Those are my books
         This is a cat
        */

        System.out.println("Hello World!");

    }
}
```

Multi-line comments are useful when a comment needs to cover multiple lines.

---

# 4. Documentation Comments

Documentation comments start with:

```java id="4v9mzo"
/**
```

and end with:

```java id="h4k2pj"
*/
```

They are mainly used to create documentation for Java code using **Javadoc**.

### Example

```java id="2aqx6r"
/**
 * Runs the Java program.
 * Prints Hello World.
 */
public static void main(String[] args) {
    System.out.println("Hello World!");
}
```

Documentation comments are commonly used for:

* Classes
* Methods
* APIs
* Libraries

---

# 5. Comments After Code

A comment can also appear after a statement.

```java id="q2z4m8"
class CommentAfterCode {
    public static void main(String[] args) {

        System.out.println("Hello World!"); // Prints Hello World

    }
}
```

The Java statement executes normally.

Only the part after `//` is treated as a comment.

---

# 6. Commenting Out Code

Comments can temporarily disable a line of code.

```java id="n8t4yv"
class CommentingCode {
    public static void main(String[] args) {

        System.out.println("Hello World!");

        // System.out.println("Hi Java!");

    }
}
```

Output:

```text id="y6a8o0"
Hello World!
```

The second `println()` does not execute because it has been commented out.

This is useful when testing or debugging code.

---

# 7. Comparing Comment Types

| Type          | Syntax   | Main Use                         |
| ------------- | -------- | -------------------------------- |
| Single-line   | `//`     | Short comments                   |
| Multi-line    | `/* */`  | Comments covering multiple lines |
| Documentation | `/** */` | Code documentation / Javadoc     |

---

# 8. Practical Example

```java id="1h9x7v"
class PracticalComments {
    public static void main(String[] args) {

        // Display the application title
        System.out.println("Student Information");

        /*
         Display basic student details.
         These values are currently hard-coded.
        */

        System.out.println("Name: Tharusha");
        System.out.println("Course: Java");

        // This line is temporarily disabled
        // System.out.println("Age: 20");

    }
}
```

Output:

```text id="q7xv5p"
Student Information
Name: Tharusha
Course: Java
```

---

# 🧪 Practice Exercises

Try these exercises without looking at the solution first.

## Exercise 01 — Single-Line Comment

Create a Java program that contains:

* One single-line comment
* One `System.out.println()` statement

Example output:

```text id="d6m1bx"
Hello Java!
```

---

## Exercise 02 — Multiple Comments

Create three different single-line comments explaining your program.

---

## Exercise 03 — Multi-Line Comment

Create a multi-line comment containing at least three lines.

Then print:

```text id="u8y2zn"
I am learning Java.
```

---

## Exercise 04 — Comment Out Code

Create three `System.out.println()` statements.

Comment out the second one.

Expected output:

```text id="j7s2pa"
Line 1
Line 3
```

---

## Exercise 05 — Comment After Code

Write three output statements and add a short comment after each statement.

Example:

```java id="v5q7xz"
System.out.println("Java"); // Programming language
```

---

## Exercise 06 — Documentation Comment

Create a simple method and add a documentation comment explaining what the method does.

---

## 🧠 Challenge

Create a small Java program that displays:

```text id="7p8z2m"
====================
   JAVA PROGRAM
====================

Name: Tharusha
Course: Java
Level: Beginner
```

Add appropriate comments explaining each section of your program.

---

# 🔍 What You Should Understand

Before moving to the next topic, make sure you can explain:

* What is a comment?
* Why are comments used?
* What does `//` mean?
* What does `/* */` mean?
* What does `/** */` mean?
* What is the difference between a normal comment and a documentation comment?
* How can you temporarily disable a line of code?
* Can comments affect program output?
* Where should useful comments be placed?

---

# ✅ Completion Checklist

* [ ] Understand single-line comments
* [ ] Understand multi-line comments
* [ ] Understand documentation comments
* [ ] Practice commenting out code
* [ ] Practice comments after statements
* [ ] Complete all exercises
* [ ] Complete the challenge
* [ ] Run and test all examples
* [ ] Commit the completed lesson to Git

---

## 🚀 Next Topic

**Variables & Data Types**

Coming next:

```text
Variables
↓
Primitive Data Types
↓
Reference Types
↓
Variable Naming Rules
↓
Declaring & Initializing Variables
↓
Practical Examples
↓
Practice Exercises
```
