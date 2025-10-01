A class in Java is a blueprint that defines what data an object can hold and what actions it can perform. You do not need to know how the computer stores the object in memory. You only need to know how to create objects from the class and use the public methods or variables it provides.

>A **class construct** is the code structure in Java that lets you define a class. It tells the compiler what data and methods belong to that class. 

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