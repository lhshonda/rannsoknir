The type of division that takes place when both [[Operand|operands]] are [[Integer (CS)|integers]]. The quotient truncates any remainder away leave an integer as the answer.

[[Integer Division (CS)|Integer division]] is not universal across [[Programming Languages|programming languages]], as some perform [[Floating-Point Division|floating-point division]] by default. 

```java
public class IntegerDivisionExample {
    public static void main(String[] args) {
        int a = 7;
        int b = 3;

        int result = a / b; // integer division
        System.out.println("7 / 3 = " + result); // output: 2

        double preciseResult = (double) a / b; // floating-point division
        System.out.println("7 / 3 as floating-point = " + preciseResult); // output: 2.3333333333333335
    }
}
```

---
#computer-science 