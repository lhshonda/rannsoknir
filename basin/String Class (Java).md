 The instances of this class, i.e. [[Object (CS)|objects]], hold text and extra details such as length. The internal structure of the class is not relevant to the programmer, rather, the point of interest lies within the 

```java
public class StringExample {
    public static void main(String[] args) {
        String name = "Honda"; // String object holds text internally

        // We do not know or care how it stores length or characters
        System.out.println(name.length());   // Get length
        System.out.println(name.toUpperCase()); // Change case
        System.out.println(name.charAt(0));  // Get first char
    }
}
```

---
#computer-science #java 