2025-09-15 // 14:11

:: [[Java]]

---

> An object's methods are commonly classified as either mutators or accessors.

A **mutator** method may modify ("mutate") the object, thereby changing the object's internal data. An **accessor** method accesses the object's data but does not modify the internal data.

---

A program uses the operations supported by objects to perform useful tasks, such as printing text or getting a user's input. A **method call** is a statement that invokes an object's method, allowing the program to perform a particular operation on that object.

Calling a method on an object requires appending the "." operator and the method's name to the object's name.

```java
objectName.methodName();
```

The "." operator is also known as the [[Member Access Operators|member access operator]].

Programmers influence the behavior of methods by providing additional input values, called **method arguments**, in a method call.

The input specified in a method definition is call a **[[Parameter|parameter]]**.

The value passed to a parameter is known as an **argument**.

```java
public class Histogram {
 
   // Internal data (private fields)
   private int[] histogramData;

   // Operations (public methods)  
   // Sets the number of bins (previous data is deleted)
   public void setNumberOfBins(int numberBins) {...}

   // Sets the value for the bin at the specified index
   public void setBinValue(int binIndex, int binValue) {...}

   // Returns the value of the bin at the specified index
   public int getBinValue(int binIndex) {...}

   // Prints the histogram
   public void printHistogram() {...}
}
```

---
##### Return Values

The type of value returned by an object's method is defined in object's class definition. A method may return a single value or none. 

A method's return value can be of any type (including a class type).

The Histogram class' getBinValue() method returns an integer value, which is specified by the int keyword before the method name in the method's declaration: 
`public int getBinValue(int binIndex) {...}`

The printHistogram() method does not return a value, specified the void in the method declaration.

A method can return either zero or one value .

---
##### Public & Private Methods

A class' **public methods** are the operations that a program can directly invoke on objects of that class type. The class' public methods are often called the class interface.

The methods for a class' interface are listed after the public keyword in the class definition. The internal data (and internal methods) are listed after the private keyword.