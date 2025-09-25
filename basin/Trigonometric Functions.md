2025-09-09 // 20:57

:: [[Mathematics]]

---

Trigonometric are **real functions** that relate an angle of a [[Right Angle|right-angled]] triangle to ratios of two side lengths. 

> Also called circular functions, angle functions or goniometric functions. An easy way to remember them is through the famous mnemonic: **SOH CAH TOA**.

$$
\begin{gather}
Sine(\sin \theta)=\frac{\text{Opposite}}{\text{Hypotenuse}}\text{ }\text{ }\text{ }\text{ } \text{Cosine}(\cos \theta)=\frac{\text{Adjacent}}{\text{Hypotenuse}}\text{ }\text{ }\text{ }\text{ } \text{Tangent}(\tan \theta)=\frac{\text{Opposite}}{\text{Adjacent}}\text{ }\text{ }\text{ } 
\end{gather}
$$

$$
\begin{gather}
\text{Cosecant}(\csc \theta)=\frac{\text{Hypotenuse}}{\text{Opposite}}\text{ }\text{ }\text{ }\text{ } \text{Secant}(\sec \theta)=\frac{\text{Hypotenuse}}{\text{Adjacent}}\text{ }\text{ }\text{ }\text{ } \text{Cotangent}(\cot \theta)=\frac{\text{Adjacent}}{\text{Opposite}}\text{ }\text{ }\text{ } 
\end{gather}
$$
---

For any right triangle, knowing how to label its sides from the perspective of $\theta$ is important.

- The hypotenuse is the longest side directly opposite of the $90^\circ$ angle.
- The opposite side is across from your angle $\theta$.
- The adjacent side is the one next to $\theta$.


```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}

\begin{tikzpicture}[
  scale=2,
  line style/.style={thick},
  label style/.style={font=\small},
  angle style/.style={font=\small, text=obsidianPurple},
  right angle style/.style={draw, thick}
]

\coordinate (A) at (0,0);
\coordinate (B) at (3,0);
\coordinate (C) at (0,2);

\draw[line style] (A) -- (B) node[midway, below, label style] {Adjacent};
\draw[line style] (A) -- (C) node[midway, left, label style] {Opposite};
\draw[line style] (B) -- (C) node[midway, above right, label style] {Hypotenuse};

\draw[right angle style] (A) ++(0,0.2) -- ++(0.2,0) -- ++(0,-0.2);

\def\endAngle{146.3}
\def\startAngle{180}
\draw[obsidianPurple, -] (B) +(\startAngle:0.5) arc (\startAngle:\endAngle:0.5);
\draw (B) + (163:0.65) node[angle style] {$\theta$};

\end{tikzpicture}
\end{document}
```
---

An abbreviation of each trigonometric function’s name is used as the symbol in formulas.

sine: `sin`
cosine: `cos`
tangent: `tan, tg`
secant: `sec`
cosecant: `csc`
cotangent:  `cot, ctg`

---

Superscripted positive integers after the symbols denote [[Exponentiation|exponentiation]], not [[Function Composition|function composition]]. In contrast, a $-1$ superscript is typically used to denote an [[Inverse Function|inverse function]] rather than a [[Reciprocal|reciprocal]].

$$
\theta=\\sin ^{-1}(x)=\\sin\ \theta=x.
$$

