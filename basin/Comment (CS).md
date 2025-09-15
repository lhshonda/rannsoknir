2025-09-15 // 13:56

:: [[Computer Science]]

---
##### Adnotanda

A comment is text a programmer adds to code, to be read by humans to better understand the code but ignored by the compiler.

---
###### Java-Specific?

- A **single-line comment** starts with // and includes all the following text on that line. Single-line comments commonly appear after a statement on the same line.
- A **multi-line comment** starts with /* and ends with */, where all text between /* and */ is part of the comment. A multi-line comment is also known as a **block comment**.

**The second // is ignored.**

```java
// Print "Hello" to the screen //
```

**Compiler errors due to second and third lines.**

```java
// Print "Hello"
   Then print "Goodbye"
   And finally return.
//
```

**The last line throws an error as it doesn't end a comment.**

```java
/* 
   numKids = 2;  /* Typical number */
   numCars = 5;
*/
```

> Java supports a third type of comment, known as a JavaDoc comment, which is a specially formatted multi-line comment that can be converted to program documentation in HTML.

