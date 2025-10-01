Whitespace refers to blank spaces (space and tab characters) between items within a statement and blank lines between statements (called newlines). A compiler ignores most whitespace.

Not all spaces are ignored by the compiler. 
Ex: The spaces in a [[String Literal|string literal]] like "Enter age: " will be printed if the string is output.

---
##### Java Specific

Good practice is to deliberately and consistently use whitespace to make a program more readable. Programmers usually follow conventions defined by their company, team, instructor, etc., such as:

- Use blank lines to separate conceptually distinct statements. 
- Indent lines the same amount.
- Align items to reduce visual clutter. 
- Use a single space before and after any operators like =, +, *, or / to make statements more readable.

**Good use of whitespace**

```java
import java.util.Scanner;

public class WhitespaceEx {
   public static void main(String[] args) {
      Scanner scnr = new Scanner(System.in);
      int myFirstVar;    // Aligned comments yield less
      int yetAnotherVar; // visual clutter
      int thirdVar;

      // Above blank line separates variable declarations from the rest
      System.out.print("Enter a number: ");
      myFirstVar = scnr.nextInt();

      // Above blank line separates user input statements from the rest
      yetAnotherVar = myFirstVar;        // Aligned = operators
      thirdVar      = yetAnotherVar + 1; 
      // Also notice the single-space on left and right of + and =
      // (except when aligning the second = with the first =)

      System.out.println("Final value is " + thirdVar); // S-Space around +
   }
}
```

---
#computer-science #java