2025-09-26 // 10:45

:: [[Java]]

---

A `String` in Java is an object that holds text and some extra details such as its length. You do not need to know how it works internally. You only need to know the public methods that let you use it.

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
