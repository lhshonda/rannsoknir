2025-09-15 // 12:48

:: [[Computer Science]]

---
##### Adnotanda

A floating-point number is a real number containing a decimal point that can appear anywhere (or "float") in the number. Ex: 98.6, 0.0001, or -55.667.

---
###### Java-Specific?

A double variable stores a floating-point number. Ex: `double milesTravel;` declares a double variable.

A floating-point [[Literal (CS)||literal]] is a number with a fractional part, even if the fraction is 0, as in 1.0, 0.0, or 99.573. Good practice is to always have a digit before the decimal point, as in 0.5, since .5 might mistakenly be viewed as 5.

A floating-point literal should have a fractional part, even if 0.

The syntax for outputting the double myFloat with two digits after the decimal point is   
`System.out.printf("%.2f", myFloat);`

---
###### Scientific Notation

Scientific notation is useful for representing floating-point numbers that are much greater than or much less than 0, such as 6.02 x 1023. A floating-point literal using scientific notation is written using an e preceding the power-of-10 exponent, as in 6.02e23 to represent 6.02 x 1023. 

The e stands for exponent. Likewise, 0.001 is 1 x 10-3 and can be written as 1.0e-3. For a floating-point literal, good practice is to make the leading digit non-zero.

###### Questions
$$
\begin{align} \\
1.0e^{-4} \neq 0.0001 \\
\text{What happened to the significance of .0?} \\
\text{If aiming to preserve all significant numbers, would it not be 0.00010 as a floating-point literal?}

\end{align}
$$
---
###### Warnings

Some programmers warn against using floating-point for money, as in 14.53 representing 14 dollars and 53 cents, because money is a countable item.