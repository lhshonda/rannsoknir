Java supports a set of objects for developing graphical applications. A graphical application is a program that displays drawings and other graphical objects.

Graphical applications display their contents inside a window called a [[Frame|frame]] using a [[JFrame]] object. The following shows how to create and configure a JFrame object to display an empty application window:

```java
import javax.swing.JFrame;

public class EmptyFrame {
   public static void main(String[] args) {
      
      // Construct the JFrame object
      JFrame appFrame = new JFrame();

      // Set the frame's width (400) and height (250) in pixels
      appFrame.setSize(400, 250);      
      // Set the frame's title
      appFrame.setTitle("An Empty Frame");      
      // Set the program to exit when the user
      // closes the frame
      appFrame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);      
      // Make the frame visible to the user
      appFrame.setVisible(true);   }
}
```

- Forgetting to set the frame's size results in a frame too small to see.

- Alternatively, the frame's title can be provided as an argument to JFrame's constructor as in `JFrame appFrame = new JFrame("An Empty Frame")`.

---
#computer-science #java