2025-09-15 // 13:05

:: [[Java]]

---
##### Adnotanda

Dividing a nonzero floating-point number by zero is undefined in regular arithmetic. Many programming languages produce an error when performing floating-point division by 0, but Java does **not**. Java handles this operation by producing **infinity or -infinity**, depending on the signs of the operands.

If the dividend and divisor in floating-point division are both 0, the division results in a "not a number". Not a number (NaN) indicates an unrepresentable or undefined value.