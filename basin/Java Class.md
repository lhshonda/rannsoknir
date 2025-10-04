[[Class (OOP)|Classes]] in Java are blueprints defining the [[Data Type (CS)|data]] their instances, [[Object (CS)|objects]] can hold and what actions they may perform.

A **class construct** is the code structure in Java that lets you define a class. It tells the [[Compiler (CS)|compiler]] what [[Data Type (CS)|data]] and [[Method (CS)|methods]] belong to that class. 

```java
// A class is a blueprint
class Car {
    // Data the object holds
    String brand;
    
    // Action the object can perform
    void honk() {
        System.out.println("Beep!");
    }
}

public class ClassExample {
    public static void main(String[] args) {
        Car myCar = new Car();   // Create an object from the class
        myCar.brand = "Honda";   // Use its data
        myCar.honk();            // Call its method
    }
}
```

---

```java
PeopleCounter passengerCounter = new PeopleCounter();
```

A `PeopleCounter` class is used to define the type of variable, in this case an object of said class, that `passengerCounter` is meant to be. 

The variable is then instantiated as an object of `PeopleCounter` through the construction call `new PeopleCounter();`.

---
#computer-science #java