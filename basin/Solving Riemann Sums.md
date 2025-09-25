2025-09-23 // 11:48

:: [[Calculus]]

---

**Finding a sum given a function**: When looking to approximate the area under a curve for any function between two intervals, you may use a number of rectangles dictated by the amount of subdivisions you look to perform.

$$
\begin{gather}
\text{In the case of } x^2+1\text{, suppose we want to utilize 4 subdivisions.} \\
\text{Furthermore we want to approximate the area between } x=1\text{, and }x=3\text{.} \\

\end{gather}
$$

In order to find the size of the subdivisions, given they're to be uniform in length, you can assume that a subdivision is the final interval position subtracted by the initial interval position over the total number of subdivisions:

$$
\begin{gather}
\Delta x= \frac{x_{f}-x_{i}}{\text{n of divisions}} = \frac{3-1}{4}=\frac{1}{2}
\end{gather}
$$

The uniform subdivisions serve as the value of the base of each rectangle. In order to find their respective height you need only to evaluate the respective boundaries based on the type of Riemann sum used. 

$$
\begin{gather}
\text{As the bases are}= \Delta x \text{, the heights are the last items of importance.} \\
\text{Solving for a left Riemann sum requires the use of the left boundaries.} \\
\\
f(1)\cdot \Delta x \:+f(1.5)\cdot \Delta x \:+f(2)\cdot \Delta x \:+f(2.5)\cdot \Delta x = \text{Approx. Area} \\ \\

\frac{1}{2}\cdot(17.5)=8.75
\end{gather}
$$

---

**Finding a sum using a table/values**: Given points $\text{(1, 6), (4, 8), (7, 3), and (10, 5).}$ Find the area underneath the curve using a [[Left & Right Riemann Sums|right Riemann sum]] with three equal subdivisions for the graph of $f$ from $x=1$ to $x=10$.

> The given points do not give an exact picture of what the function might look like on the graph. This, however, does not prevent us from performing an approximation utilizing a Riemann sum.

- Since we are solving for the right Riemann sum, we look to use the right boundary of the subdivisions provided.

$$
\begin{gather}
\text{The sum is simply the added area of the provided rectangles in respect to direction.} \\
\text{The heights 8, 3, and 5 are used. All rectangles have a base of 3 here.} \\ (3\cdot 8)+(3\cdot 3)+(3\cdot 5) = 48

\end{gather}
$$

> This approximation isn't inherently bad or good without an understanding of the nature of $f$ in its entirety. 

---

