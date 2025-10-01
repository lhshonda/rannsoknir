A two [[Dimension|dimensional]] space created by the intersection of two [[Perpendicular|perpendicular]] lines. These lines are the axes and their intersection creates the [[Origin|origin]].

The division created by the two lines create four separate regions named [[Quadrants|quadrants]].


```tikz
\begin{document}

\usetikzlibrary{arrows.meta}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\definecolor{obsidianGreen}{rgb}{0.455,0.639,0.036}

\begin{tikzpicture}[
  scale=1.2,
  every node/.style={font=\small},
  axis style/.style={->, gray!70, thick, -{Latex[length=2.5mm]}},
  label style/.style={font=\large}
]


\draw[axis style] (-3.5,0) -- (3.5,0) node[right] {$x$-axis};

\draw[axis style] (0,-3.5) -- (0,3.5) node[above] {$y$-axis};


\fill[obsidianPurple] (0,0) circle (1.5pt);
\node[below left, obsidianPurple] at (-0.1,-0.1) {Origin $(0,0)$};


\node[label style] at (2,2) {Quadrant I};
\node[label style] at (2,1.5) {$(+x, +y)$};
\node[label style] at (-2,2) {Quadrant II};
\node[label style] at (-2,1.5) {$(-x, +y)$};
\node[label style] at (-2,-2) {Quadrant III};
\node[label style] at (-2,-1.5) {$(-x, -y)$};
\node[label style] at (2,-2) {Quadrant IV};
\node[label style] at (2,-1.5) {$(+x, -y)$};

\end{tikzpicture}
\end{document}
```

---
#math 