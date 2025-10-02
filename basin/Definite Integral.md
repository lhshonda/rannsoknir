Formally defined as the limit of a [[Riemann Sum|Riemann sum]]. The notation commands: find the exact area under the curve of $f(x)$ from $x=a$ to $x=b$.

```tikz
\begin{document}

\usetikzlibrary{arrows.meta}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\definecolor{obsidianGreen}{rgb}{0.455,0.639,0.036}

\begin{tikzpicture}[
  scale=1.5,
  every node/.style={font=\small},
  axis style/.style={-Stealth, gray!70, thick},
  line style/.style={thick, obsidianPurple},
  label style/.style={font=\large},
  declare function={f(\x) = (\x-1.5)^2 * 0.4 + 1;}
]


\draw[axis style] (-0.5,0) -- (5.5,0) node[right] {$x$};
\draw[axis style] (0,-0.5) -- (0,4.5) node[above] {$y$};


\draw[line style, domain=0:5] plot (\x, {f(\x)});
\node[right, text=obsidianPurple!70] at (5, {f(5)}) {$f(x)$};


\def\a{1}
\def\b{4}


\fill[ opacity=0.3] plot[domain=\a:\b] (\x, {f(\x)}) -- (\b,0) -- (\a,0) -- cycle;


\draw[dashed, gray!30] (\a,0) node[below] {$a$} -- (\a, {f(\a)});
\draw[dashed, gray!30] (\b,0) node[below] {$b$} -- (\b, {f(\b)});


\end{tikzpicture}
\end{document}
```

$$
\begin{gather}
\int_{a}^{b}f(x)dx \\ \\
\small{\int} \to\text{ Symbol for Integration} \\ \\
\small\text{a \& b } \to \text{ Limits of Itegration} \\ \\
\small f(x) \to \text{ The Integrand} \\ \\
\small dx \to \text{Variable of Integration} \\
\end{gather}
$$
---
#math #calculus 