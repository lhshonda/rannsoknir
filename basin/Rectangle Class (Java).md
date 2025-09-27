2025-09-15 // 15:03

:: [[Java Class]]

---

The Java Rectangle class contains four instance members for the X and Y location of the rectangle's upper left corner, the rectangle's width, and the rectangle's height.

```java
new Rectangle(40, 80, 100, 120)
```

This set of arguments creates a `Rectangle` with the upper left corner at location (40, 80) and with a size that is 100 units wide by 120 units high.

---

The Rectangle class has **mutator methods** to manipulate a rectangle's size and location.
- The setSize(width, height) method changes the width and height.
- The setLocation(xLoc, yLoc) method changes the location of the upper left corner.
- The translate(xDist, yDist) method repositions the Rectangle by the specified distances in the X and Y direction.

```java
translate(30, 40)
```

This moves the rectangle to the right 30 units and downward 40 units.
The Java coordinate system places the origin (0, 0) in the upper left corner