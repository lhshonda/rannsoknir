The concepts of **accuracy** and **precision** are independent, yet complementary. 

```tikz

\begin{document}
\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\begin{tikzpicture}[
    scale=0.8,
    every node/.style={font=\small},
    target ring/.style={draw, thick, circle, gray!70},
    shot marker/.style={fill=obsidianPurple!70, draw=obsidianPurple},
    label style/.style={font=\large}
]

\begin{scope}[shift={(-3,0)}]
    \draw (0, -2.5) node[label style] {High Accuracy, High Precision};
    \draw[target ring] (0,0) circle (2);
    \draw[target ring] (0,0) circle (1.5);
    \draw[target ring] (0,0) circle (1);
    \draw[target ring] (0,0) circle (0.5);
    \fill[shot marker] (0.1, 0.1) circle (2pt);
    \fill[shot marker] (-0.1, -0.1) circle (2pt);
    \fill[shot marker] (0.05, -0.15) circle (2pt);
    \fill[shot marker] (-0.05, 0.15) circle (2pt);
\end{scope}


\begin{scope}[shift={(6,0)}]
    \draw (0, -2.5) node[label style] {Low Accuracy, High Precision};
    \draw[target ring] (0,0) circle (2);
    \draw[target ring] (0,0) circle (1.5);
    \draw[target ring] (0,0) circle (1);
    \draw[target ring] (0,0) circle (0.5);
    \fill[shot marker] (1.5, 1.5) circle (2pt);
    \fill[shot marker] (1.6, 1.4) circle (2pt);
    \fill[shot marker] (1.4, 1.6) circle (2pt);
    \fill[shot marker] (1.55, 1.55) circle (2pt);
\end{scope}


\begin{scope}[shift={(-3,-6)}]
    \draw (0, -2.5) node[label style] {High Accuracy, Low Precision};
    \draw[target ring] (0,0) circle (2);
    \draw[target ring] (0,0) circle (1.5);
    \draw[target ring] (0,0) circle (1);
    \draw[target ring] (0,0) circle (0.5);
    \fill[shot marker] (1.5, 0) circle (2pt);
    \fill[shot marker] (-1.5, 0) circle (2pt);
    \fill[shot marker] (0, 1.5) circle (2pt);
    \fill[shot marker] (0, -1.5) circle (2pt);
\end{scope}


\begin{scope}[shift={(6,-6)}]
    \draw (0, -2.5) node[label style] {Low Accuracy, Low Precision};
    \draw[target ring] (0,0) circle (2);
    \draw[target ring] (0,0) circle (1.5);
    \draw[target ring] (0,0) circle (1);
    \draw[target ring] (0,0) circle (0.5);
    \fill[shot marker] (1.7, -1.2) circle (2pt);
    \fill[shot marker] (-0.5, 1.8) circle (2pt);
    \fill[shot marker] (-1.8, -1.0) circle (2pt);
    \fill[shot marker] (0.2, -1.9) circle (2pt);
\end{scope}

\end{tikzpicture}
\end{document}
```

---
#physics 