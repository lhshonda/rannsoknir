Contains roughly 30 operations known as methods. No import is required as it's in Java's standard language pack.

```java
public class LabProgram {
   public static void main(String[] args) {
      double x = 9.0;
      double y = -3.7;

      // Square root
      System.out.println("sqrt(9.0) = " + Math.sqrt(x));

      // Power
      System.out.println("2^3 = " + Math.pow(2, 3));

      // Absolute value
      System.out.println("abs(-3.7) = " + Math.abs(y));

      // Maximum and minimum
      System.out.println("max(9.0, -3.7) = " + Math.max(x, y));
      System.out.println("min(9.0, -3.7) = " + Math.min(x, y));

      // Rounding
      System.out.println("round(3.7) = " + Math.round(3.7));
      System.out.println("floor(3.7) = " + Math.floor(3.7));
      System.out.println("ceil(3.7) = " + Math.ceil(3.7));

      // Trigonometry (Math uses radians)
      System.out.println("sin(π/2) = " + Math.sin(Math.PI / 2));
   }
}
```

---
#computer-science #java 