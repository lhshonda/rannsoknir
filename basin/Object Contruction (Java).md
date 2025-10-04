Creating an object and assigning a variable with that object involves three parts: 

```java
Histogram passFailHistogram = new Histogram();
```

**Variable declaration**: A reference is a variable type that refers to an object. A reference may be thought of as storing the memory address of an object. 

```java
Histogram passFailHistogram
```

 **Memory allocation**: The `new` operator creates an object by allocating memory for the object and initializing the object by calling a constructor.

```java
new
```

**Calling the constructor**: A constructor is a special method for an object that is called whenever a new object is created, and is used to initialize the object's internal data. A class may define more than one constructor. The `Histogram()` part of the statement indicates which constructor should be called.

```java
Histogram();
```

---
#computer-science #java