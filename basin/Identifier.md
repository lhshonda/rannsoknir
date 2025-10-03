The name assigned to elements such as variables, methods, classes, or objects.  They can include letter, digits, underscores, and dollar signs. Identifiers may **not** start with digits. 

Most identifiers begin with a letter and follow the [[Camel Case|camelCase]] naming style for variables and methods, and [[Pascal Case|PascalCase]] for classes. Identifiers share some conventions across languages, but this isn't always the case, and it's best you consult the appropriate documentation.

```java
public class IdentifierExample {
   public static void main(String[] args) {
      int age = 20;          // valid identifier
      double _salary = 5000; // valid, but underscore start is unusual
      String $name = "Alex"; // valid, but dollar sign is uncommon
      
      // int 2cool = 5;      // invalid: cannot start with a digit
      
      System.out.println(age);
      System.out.println(_salary);
      System.out.println($name);
   }
}
```

---
#computer-science 