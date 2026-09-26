# ☕ Java Output — Beginner Practice

This section introduces the basics of displaying output in Java using `System.out.print()` and `System.out.println()`.

The goal is to understand how Java displays text, numbers, spaces, and special characters on the console.

---

## 📚 Learning Objectives

By completing this section, you should understand:

* `System.out.print()`
* `System.out.println()`
* Difference between `print()` and `println()`
* Printing multiple values
* New lines using `\n`
* Tab spaces using `\t`
* Escape sequences
* Printing special characters
* Basic output formatting
* Creating simple patterns using output statements

---

# 1. `System.out.print()`

`System.out.print()` displays the given value on the console without moving to the next line.

### Example

```java
class Print01 {
    public static void main(String[] args) {
        System.out.print("Hello, World!");
    }
}
```

### Output

```text
Hello, World!
```

---

## Multiple `print()` Statements

```java
class Print02 {
    public static void main(String[] args) {
        System.out.print("Hello ");
        System.out.print("Java ");
        System.out.print("Programming");
    }
}
```

### Output

```text
Hello Java Programming
```

All three outputs are displayed on the **same line**.

---

# 2. `System.out.println()`

`System.out.println()` displays the given value and then moves the cursor to the next line.

### Example

```java
class Println01 {
    public static void main(String[] args) {
        System.out.println("Hello");
        System.out.println("Java");
        System.out.println("Programming");
    }
}
```

### Output

```text
Hello
Java
Programming
```

Each `println()` statement starts the next output on a new line.

---

# 3. `print()` vs `println()`

| Method      | Behaviour                         |
| ----------- | --------------------------------- |
| `print()`   | Prints and stays on the same line |
| `println()` | Prints and moves to the next line |

### Example

```java
class PrintVsPrintln01 {
    public static void main(String[] args) {
        System.out.print("ABC");
        System.out.println("DEF");
        System.out.print("GHI");
    }
}
```

### Output

```text
ABCDEF
GHI
```

### How it works

```text
print("ABC")     → ABC
println("DEF")   → DEF + next line
print("GHI")     → GHI
```

---

# 4. Printing Different Types of Values

Java output methods can also display numbers and boolean values.

```java
class PrintValues {
    public static void main(String[] args) {
        System.out.println("Chathumi");
        System.out.println(100);
        System.out.println(25.5);
        System.out.println(true);
    }
}
```

### Output

```text
Chathumi
100
25.5
true
```

---

# 5. New Line Using `\n`

`\n` is an escape sequence used to move the output to a new line.

```java
class NewLine01 {
    public static void main(String[] args) {
        System.out.print("Hello\nJava");
    }
}
```

### Output

```text
Hello
Java
```

Multiple new lines can also be used:

```java
System.out.print("A\nB\nC\nD");
```

Output:

```text
A
B
C
D
```

---

# 6. Tab Using `\t`

`\t` inserts a tab space.

```java
class Escape01 {
    public static void main(String[] args) {
        System.out.println("Name:\tChathumi");
        System.out.println("Age:\t21");
        System.out.println("Course:\tICT");
    }
}
```

### Output

```text
Name:   Chathumi
Age:    21
Course: ICT
```

---

# 7. Printing Double Quotes

A double quote inside a Java string needs to be escaped using `\"`.

```java
class Escape02 {
    public static void main(String[] args) {
        System.out.println("He said \"Hello Java\"");
    }
}
```

### Output

```text
He said "Hello Java"
```

---

# 8. Printing a Backslash

A backslash can be printed using `\\`.

```java
class Escape03 {
    public static void main(String[] args) {
        System.out.println("C:\\Java\\Projects");
    }
}
```

### Output

```text
C:\Java\Projects
```

---

# 9. Simple Star Patterns

Output statements can be used to create simple patterns.

### Pattern 01

```text
*
**
***
****
*****
```

Example:

```java
class Pattern01 {
    public static void main(String[] args) {
        System.out.println("*");
        System.out.println("**");
        System.out.println("***");
        System.out.println("****");
        System.out.println("*****");
    }
}
```

---

### Pattern 02

```text
*****
****
***
**
*
```

---

### Pattern 03

```text
    *
   ***
  *****
 *******
```

---

### Pattern 04 — Diamond

```text
   *
  ***
 *****
*******
 *****
  ***
   *
```

---

### Pattern 05 — Number Pattern

```text
1
12
123
1234
12345
```

---

### Pattern 06 — Character Pattern

```text
A
AB
ABC
ABCD
ABCDE
```

---

# 📝 Practice Exercises

Try these exercises **without looking at the solution first**.

## Exercise 01 — Personal Information

Print your:

* Name
* Age
* City
* Course

Each item should appear on a separate line.

Expected output:

```text
Name: Chathumi
Age: 21
City: Galle
Course: ICT
```

---

## Exercise 02 — Same Line

Print the following output using `System.out.print()`:

```text
Hello Java Programming
```

Use multiple `print()` statements.

---

## Exercise 03 — Separate Lines

Print:

```text
Java
Python
C
JavaScript
```

Use `System.out.println()`.

---

## Exercise 04 — Print vs Println

Predict the output before running this code:

```java
System.out.print("A");
System.out.println("B");
System.out.print("C");
System.out.println("D");
```

Then run the program and compare your answer.

---

## Exercise 05 — New Line

Print the following using `\n`:

```text
Java
is
easy
to
learn
```

---

## Exercise 06 — Tab

Print the following using `\t`:

```text
Name:    Chathumi
Course:  ICT
```

---

## Exercise 07 — Quotes

Print exactly:

```text
Java is called "Write Once, Run Anywhere".
```

Use an escape sequence.

---

## Exercise 08 — File Path

Print:

```text
C:\Users\Chathumi\Java
```

Use the correct escape sequence for the backslashes.

---

## Exercise 09 — Star Pattern

Create:

```text
*
**
***
****
*****
```

---

## Exercise 10 — Reverse Star Pattern

Create:

```text
*****
****
***
**
*
```

---

## Exercise 11 — Pyramid

Create:

```text
    *
   ***
  *****
 *******
```

Pay attention to the spaces.

---

## Exercise 12 — Diamond

Create:

```text
   *
  ***
 *****
*******
 *****
  ***
   *
```

---

# 🧠 Challenge

Try to create this output using only `System.out.print()` and `System.out.println()`:

```text
====================
   JAVA PROGRAMMING
====================

Name: Chathumi
Course: ICT
City: Galle

Learning Java is fun!
```

Try to create it **without using variables**.

---

# 🔍 What You Should Understand

Before moving to the next topic, make sure you can explain:

* What does `System.out` mean?
* What does `print()` do?
* What does `println()` do?
* What is the difference between `print()` and `println()`?
* What does `\n` do?
* What does `\t` do?
* Why do we use `\"`?
* Why do we use `\\`?
* How can spaces be used to create patterns?
* How can multiple output statements create a pattern?

---

# 🎯 Learning Flow

```text
Theory
   ↓
Examples
   ↓
Run the Code
   ↓
Predict the Output
   ↓
Practice Exercises
   ↓
Pattern Challenges
   ↓
Understand the Output
   ↓
Git Commit
```

---

# ✅ Completion Checklist

* [ ] Understand `System.out.print()`
* [ ] Understand `System.out.println()`
* [ ] Understand `print()` vs `println()`
* [ ] Practice `\n`
* [ ] Practice `\t`
* [ ] Practice `\"`
* [ ] Practice `\\`
* [ ] Complete output exercises
* [ ] Complete star patterns
* [ ] Complete number/character patterns
* [ ] Complete the challenge
* [ ] Commit the completed lesson to Git

---

## 🚀 Next Topic

After completing Output, move to:

**03 — Variables & Data Types**

Topics will include:

* Variables
* Variable declaration
* Variable initialization
* Primitive data types
* Reference types
* Naming rules
* Basic variable usage
