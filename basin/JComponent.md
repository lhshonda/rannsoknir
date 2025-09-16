2025-09-15 // 23:41

:: [[Java]]

---

A JComponent is a blank graphical component that a programmer extends (or customizes) with custom code in order to draw basic shapes.

The code below demonstrates how to create a custom class that extends JComponent to draw 2D graphics:

```java
import java.awt.Graphics;
import java.awt.Graphics2D;
import javax.swing.JComponent;

public class MyCustomJComponent extends JComponent {

   @Override
   public void paintComponent(Graphics g) {
      // Cast to Graphics2D
      Graphics2D graphicsObj = (Graphics2D)g;

      // Write your drawing instructions
   }
}
```

The above code defines a [[Class (Programming)|class]] named MyCustomJComponent that extends JComponent. 
The class should be saved to a separate file named with the same name:

`MyCustomJComponent.java` 

A programmer completes the template by providing custom drawing instructions in the paintComponent() method.

---

> Drawing a histogram in a frame.

```java
import java.awt.Color;
import java.awt.Graphics;
import java.awt.Graphics2D;
import java.awt.Rectangle;
import javax.swing.JComponent;

// HistogramComponent extends the functionality of a JComponent
// in order to draw a histogram.
public class HistogramComponent extends JComponent {
   
   // Paints a histogram with three bins
   @Override
   public void paintComponent(Graphics g) {  
      // 1. Cast to Graphics2D
      Graphics2D graphicsObj = (Graphics2D) g;
      
      // Draw 1st bin as an olive colored rectangle at (10,10)
      // with width = 200 and height = 50
      // 2. Create a Rectangle object
      Rectangle binRectangle1 = new Rectangle(10, 10, 200, 50);
      // 3. Create a Color object
      Color binColor1 = new Color(128, 128, 0);
      // 4. Set the color used by the Graphics2D object
      graphicsObj.setColor(binColor1);
      // 5. Draw the shape
      graphicsObj.fill(binRectangle1);
      
      // Draw 2nd bin as a teal blue rectangle at (10,75)
      // with width = 150 and height = 50
      Rectangle binRectangle2 = new Rectangle(10, 75, 150, 50); 
      Color binColor2 = new Color(0, 200, 200);
      graphicsObj.setColor(binColor2);
      graphicsObj.fill(binRectangle2);
      
      // Draw 3rd bin as a gray rectangle at (10,140)
      // with width = 350 and height = 50
      Rectangle binRectangle3 = new Rectangle(10, 140, 350, 50); 
      Color binColor3 = new Color(100, 100, 100);
      graphicsObj.setColor(binColor3);
      graphicsObj.fill(binRectangle3);
   }
}
```

The HistogramComponent's paintComponent() uses Rectangle and Color objects to draw a simple histogram with three bins, using the operations:

1. **Cast the Graphics object to Graphics2D**: The statement `Graphics2D graphicsObj = (Graphics2D) g;` converts the original Graphics object argument to a graphics object that supports drawing two-dimensional objects.
2. **Create a Rectangle object**: A Rectangle object stores the location and size of a rectangle shape. A Rectangle's constructor accepts arguments for location and size (in pixel units) as specified by the constructor definition: `Rectangle(int x, int y, int width, int height
3. **Create a Color object**: A Color object represents a color in the red, green, blue color space. A Color constructor accepts an integer value between 0 to 255 for each color channel as specified by the constructor definition: `Color(int red, int green, int blue)`. For example, the statement  `Color binColor1 = new Color(128, 128, 0);`creates a Color object with an olive color.
4. **Set the color used by the Graphics2D object**: Graphic2D's setColor() method sets the color that the Graphics2D object will use for subsequent drawing operations.
5. **Draw the shape**: A Graphic2D object provides different methods for drawing shapes. The draw() method will draw an outline of a shape, such as a Rectangle object, using the Graphic2D object's current color. The fill() method will draw a shape filling the interior of the shape with the Graphic2D object's current color.