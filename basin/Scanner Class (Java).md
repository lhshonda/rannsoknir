2025-09-10 // 12:04

:: [[Java Classes]]

##### Adnotanda

Scanner's nextDouble() method reads a floating-point value from input. 

Ex: `currentTemp = scnr.nextDouble();` reads a floating-point value from the input and assigns currentTemp with that value.

```java
import java.util.Scanner;

public class TravelTime {
   public static void main(String[] args) {
      Scanner scnr = new Scanner(System.in);
      double milesTravel; // User input of miles to travel
      double hoursFly;    // Travel hours if flying those miles
      double hoursDrive;  // Travel hours if driving those miles

      System.out.print("Enter distance in miles: ");
      milesTravel = scnr.nextDouble();

      hoursFly   = milesTravel / 500.0;
      hoursDrive = milesTravel / 60.0;

      System.out.println(milesTravel + " miles would take:");
      System.out.println("   " + hoursFly + " hours to fly,");
      System.out.println("   " + hoursDrive + " hours to drive.");
   }
}
```
