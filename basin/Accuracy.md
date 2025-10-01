This refers to distance a set of measurements are from the true value. See [[Accuracy & Precision in Tandem|this figure]] to observe how accuracy and precision relate. 

```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\definecolor{obsidianGreen}{rgb}{0.455,0.639,0.036}

\begin{tikzpicture}[
    scale=1.2,
    every node/.style={font=\small},
    axis style/.style={thick, gray!70},
    true value style/.style={ultra thick},
    measurement style/.style={fill=obsidianPurple!70, draw=obsidianPurple},
    title style/.style={font=\large}
]


\begin{scope}[shift={(0,3)}]
    \draw[axis style] (0,0) -- (6,0);
    \draw[true value style] (3,-0.2) -- (3,0.2) node[above=4pt] {True Value};
    
    \fill[measurement style] (2.8, 0) circle (2pt);
    \fill[measurement style] (3.3, 0) circle (2pt);
    \fill[measurement style] (2.9, 0) circle (2pt);
    \fill[measurement style] (3.1, 0) circle (2pt);
    
    \draw (3, -0.8) node[title style] {High Accuracy};
\end{scope}


\begin{scope}[shift={(0,0)}]
    \draw[axis style] (0,0) -- (6,0);
    \draw[true value style] (3,-0.2) -- (3,0.2) node[above=4pt] {True Value};
    
    \fill[measurement style] (4.8, 0) circle (2pt);
    \fill[measurement style] (5.3, 0) circle (2pt);
    \fill[measurement style] (4.9, 0) circle (2pt);
    \fill[measurement style] (5.1, 0) circle (2pt);

    \draw (3, -0.8) node[title style] {Low Accuracy};
\end{scope}

\end{tikzpicture}
\end{document}
```

---
#physics 