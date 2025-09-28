2025-09-23 // 11:48

:: [[Calculus]]

---

A Riemann Sum is an approximation of the area under a curve. There are different types of Riemann sums. They use a finite, countable number of rectangles.

$$
Area≈\sum_{i=1}^{n}f(x_{i}^{*})\Delta x
$$

---

>Left & Right Endpoint Summations

```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}

\begin{tikzpicture}[
    scale=0.8,
    every node/.style={font=\small},
    axis style/.style={->, gray!20, thick},
    curve style/.style={thick},
    rectangle style/.style={draw=obsidianPurple, dashed},
    label style/.style={font=\small},
    title style/.style={font=\large}
]


\begin{scope}[shift={(0,0)}]

    \draw[axis style] (0,0) -- (4.5,0) node[right] {$x$}; 
    \draw[axis style] (0,0) -- (0,4.5) node[above] {$y$}; 
    \draw[curve style] plot[domain=0:4, samples=50] (\x, {0.5*\x + 1});


    \foreach \i in {0,1,2,3} {
        \pgfmathsetmacro{\xcurr}{\i}
        \pgfmathsetmacro{\xnext}{\i+1}
        \pgfmathsetmacro{\height}{0.5*\xcurr + 1} 
        \draw[rectangle style] (\xcurr, 0) rectangle (\xnext, \height);
    }

    \draw (2.25, -1.0) node[title style] {Left Riemann Sum};
\end{scope}


\begin{scope}[shift={(7.5,0)}] 
    
    \draw[axis style] (0,0) -- (4.5,0) node[right] {$x$}; 
    \draw[axis style] (0,0) -- (0,4.5) node[above] {$y$}; 
    \draw[curve style] plot[domain=0:4, samples=50] (\x, {0.5*\x + 1});


    \foreach \i in {1,2,3,4} {
        \pgfmathsetmacro{\xprev}{\i-1}
        \pgfmathsetmacro{\xcurr}{\i}
        \pgfmathsetmacro{\height}{0.5*\xcurr + 1} 
        \draw[rectangle style] (\xprev, 0) rectangle (\xcurr, \height);
    }

    \draw (2.25, -1.0) node[title style] {Right Riemann Sum};
\end{scope}

\end{tikzpicture}
\end{document}
```

---

**Finding a sum given a function**: When looking to approximate the area under a curve for any function between two intervals, you may use a number of rectangles dictated by the amount of subdivisions you look to perform.

>Riemann sums contain what we refer to as subdivisions/partitions. These terms refer the amount of rectangles used, or rather the number of parts the interval being measured was divided into.

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

The uniform subdivisions serve as the value of each rectangle's base. The heights used to calculate the area under the curve depend on the type of Riemann sum used. 

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

**Finding a sum using a table/values**: Given points $\text{(1, 6), (4, 8), (7, 3), and (10, 5).}$ Find the area underneath the curve using a right Riemann sum with three equal subdivisions for the graph of $f$ from $x=1$ to $x=10$.

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

