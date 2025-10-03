A variable (usually initialized) whose value cannot be changed. Also known as final variable. It's common convention to name a constant variable with `UPPER_CASE` letters separated by underscore in order to make it identifiable.

```java
public class TemperatureConverter {

   // Constants for conversion formula
   public static final double NINE_OVER_FIVE = 9.0 / 5.0;
   public static final double FREEZING_POINT_F = 32.0;

   public static double celsiusToFahrenheit(double celsius) {
      return (celsius * NINE_OVER_FIVE) + FREEZING_POINT_F;
   }

   public static void main(String[] args) {
      double c1 = 0.0;   // freezing point
      double c2 = 100.0; // boiling point

      System.out.println("0°C = " + celsiusToFahrenheit(c1) + "°F");
      System.out.println("100°C = " + celsiusToFahrenheit(c2) + "°F");
   }
}
```

---
#computer-science 