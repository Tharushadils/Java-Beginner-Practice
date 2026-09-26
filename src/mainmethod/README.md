# ☕ Java Main Method — Beginner Course

This is a beginner-friendly Java practice lesson focused on understanding the `main()` method, its syntax, and different valid and invalid method declarations.

## 🎯 Learning Objectives

By completing this lesson, you will understand:

* What the `main()` method is
* Why Java applications use `main()` as an entry point
* What `public`, `static`, and `void` mean
* Why `String[] args` is used
* Which parts of the `main()` declaration can be changed
* The difference between valid and invalid method declarations
* How Java identifies the application entry point

---

## 1. What is the `main()` Method?

The `main()` method is the starting point of a standard Java application.

```java
class Main {
    public static void main(String[] args) {
        System.out.print("Hello, World!");
    }
}
```

When the Java program starts, the JVM looks for a suitable `main()` method to begin execution.

---

## 2. Understanding the Syntax

```java
public static void main(String[] args)
```

### `public`

Allows the JVM to access the method from outside the class.

### `static`

Allows the JVM to call the method without creating an object of the class.

### `void`

Means the method does not return a value.

### `main`

This is the special method name recognized as the application entry point.

### `String[]`

Represents an array of `String` values.

### `args`

This is the parameter name.

The parameter name does **not** have to be `args`.

For example, these are valid:

```java
String[] args
String[] kamal
String[] hasitha
String[] chathunga
```

---

## 3. Valid Main Method Variations

Java allows some variations in the declaration while keeping the required method characteristics.

### Variation 1

```java
public static void main(String[] args)
```

### Variation 2

```java
public static void main(String [] args)
```

### Variation 3

```java
public static void main(String... args)
```

### Variation 4

```java
public static void main(String args[])
```

The parameter name can also be changed:

```java
public static void main(String[] kamal)
```

```java
public static void main(String[] hasitha)
```

```java
public static void main(String[] chathunga)
```

---

## 4. Why Can the Parameter Name Change?

Because `args` is only a variable name.

For example:

```java
public static void main(String[] args)
```

and

```java
public static void main(String[] studentNames)
```

have the same parameter type:

```text
String[]
```

Only the variable name is different.

---

## 5. Invalid Main Method Examples

The following examples do not provide the required Java application entry point.

### Missing `[]`

```java
public static void main(String args)
```

Here, the parameter is a single `String`, not a `String[]`.

### Wrong parameter type

```java
public static void main(int[] args)
```

The parameter type is `int[]` instead of `String[]`.

### Missing `static`

```java
public void main(String[] args)
```

This is an instance method, not the required static entry point.

### Missing `public`

```java
static void main(String[] args)
```

The method is not declared `public`.

---

## 6. Illegal Java Syntax

Some declarations are not even valid method declarations.

### Wrong capitalization

```java
public static void main(string[] args)
```

Java is case-sensitive.

`String` and `string` are different identifiers.

### Missing return type

```java
public static main(String[] args)
```

A method declaration requires a return type such as:

```java
void
int
double
String
```

### Invalid method declaration

```java
public static void(String[] args)
```

A method must have a method name.

---

## 7. Important Rule

A commonly used Java application entry point is:

```java
public static void main(String[] args)
```

Remember these key points:

```text
public  → accessible
static  → no object required
void    → no return value
main    → entry-point method name
String[] → parameter type
args    → parameter name
```

---

## 🧪 Practice

Try creating your own valid versions of the `main()` method.

### Challenge 01

Change the parameter name:

```java
public static void main(String[] __________) {
}
```

### Challenge 02

Try different valid placements of `[]`.

### Challenge 03

Create three invalid versions and explain why each one is invalid.

### Challenge 04

Run each example and observe which ones compile and which ones don't.

---

## 📚 What You Learn From This Repository

This repository is not only about memorizing the `main()` method.

The goal is to learn how small changes in Java syntax can affect:

* Compilation
* JVM execution
* Method declarations
* Parameters
* Access modifiers
* Static methods
* Return types

More Java beginner topics will be added progressively.

---
## 🚀 Next Topic

**Output**

Coming next:

```text
System.out.print()
↓
System.out.println()
↓
print() vs println()
↓
New Lines & Escape Sequences
↓
Output Formatting
↓
Simple Patterns
↓
Practice Exercises
```
