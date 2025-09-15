2025-09-15 // 10:43

:: [[Computer Science]]

---
##### Adnotanda

An expression is evaluated using the order of standard mathematics, such order known in programming as precedence rules, listed below.

| Operator/Convention |                                            Description                                             |                                                                                          Explanation                                                                                           |
|:-------------------:|:--------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|         ( )         |                            Items within parentheses are evaluated first                            |                                                      In 2 * (x + 1), the x + 1 is evaluated first, with the result then multiplied by 2.                                                       |
|     **unary -**     |                             - used for negation (unary minus) is next                              |                                                           In 2 * -x, the -x is computed first, with the result then multiplied by 2.                                                           |
|      *** / %**      |                   Next to be evaluated are *, /, and %, having equal precedence.                   |                                                                                   (% is discussed elsewhere)                                                                                   |
|       **+ -**       |                            Finally come + and - with equal precedence.                             | In y = 3 + 2 * x, the 2 * x is evaluated first, with the result then added to 3, because * has higher precedence than +. Spacing doesn't matter: y = 3+2 * x would still evaluate 2 * x first. |
|  **left-to-right**  | If more than one operator of equal precedence could be evaluated, evaluation occurs left to right. |                                                       In y = x * 2 / 3, the x * 2 is first evaluated, with the result then divided by 3.                                                       |