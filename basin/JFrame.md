A JFrame can be used to draw graphical objects, such as rectangles, circles, and lines. To display graphical objects, a programmer can add a _custom_ [[JComponent]] object to a frame.

```java
import javax.swing.*;
import java.awt.*;

public class SimpleDrawing {

   // Custom JComponent
   static class MyCanvas extends JComponent {
      @Override
      public void paintComponent(Graphics g) {
         super.paintComponent(g);

         // Draw a rectangle
         g.setColor(Color.BLUE);
         g.fillRect(50, 50, 100, 60);

         // Draw a circle
         g.setColor(Color.RED);
         g.fillOval(200, 50, 80, 80);

         // Draw a line
         g.setColor(Color.BLACK);
         g.drawLine(50, 150, 280, 150);
      }
   }

   public static void main(String[] args) {
      JFrame frame = new JFrame("Drawing Example");
      frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
      frame.setSize(400, 300);

      // Add the custom component
      frame.add(new MyCanvas());

      frame.setVisible(true);
   }
}
```

---
#computer-science #java