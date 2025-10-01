To be **constant** implies a state of invariance. [[Coefficient|Coefficients]] embedded within polynomial [[Mathematical Expression|expressions]] would classify as constants. A [[Function|function]] of fixed value would be considered a constant.

```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}

\begin{tikzpicture}[
  scale=1.5,
  every node/.style={font=\small},
  axis style/.style={->, gray!70, thick},
  line style/.style={thick, obsidianPurple},
  label style/.style={font=\large},
  constant value style/.style={font=\large}
]


\draw[axis style] (-1,0) -- (4,0) node[right] {$x$};
\draw[axis style] (0,-1) -- (0,3) node[above] {$y$};


\def\constantValue{1.5}
\draw[line style] (-0.8, \constantValue) -- (3.8, \constantValue);


\draw (3.5, \constantValue) node[above right, label style, obsidianPurple!70] {$y = b$};


\draw[fill=obsidianPurple!70, obsidianPurple!70] (0, \constantValue) circle (1.5pt) node[left=3pt, constant value style, above left, obsidianPurple!70] {$b$};


\draw[dashed, gray!50] (1,0) -- (1,\constantValue);
\draw[dashed, gray!50] (2.5,0) -- (2.5,\constantValue);

\end{tikzpicture}
\end{document}
```
$$
\begin{gather}
\text{Regardless of change in the }x\text{-axis, the function output remains the same.} \\
y=c\text{ }\text{ }\text{is therefore, a constant function.}
\end{gather}
$$
---
#math

