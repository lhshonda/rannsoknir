A system that specifies each point as a pair of [[Real Number|real numbers]] called coordinates.

---
##### Basketball Through a Hoop

Imagine a graph defined with specific points. The coordinate system makes up the ball's position, while each point defines a time instance.


```tikz
\begin{document}

\usetikzlibrary{calc,arrows.meta}
\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\definecolor{obsidianGreen}{rgb}{0.455,0.639,0.036}

\begin{tikzpicture}[
  scale=1.2,
  every node/.style={font=\small},
  axis style/.style={->, gray!70, thick},
  path style/.style={-Stealth,thick, obsidianPurple},
  vector style/.style={-Stealth, thick, obsidianGreen},
  label style/.style={font=\small},
  point label style/.style={font=\small, text=obsidianPurple!70}
]


\draw[axis style] (0,0) -- (7,0) node[right] {$x$ (m)};
\draw[axis style] (0,0) -- (0,6) node[above] {$y$ (m)};


\draw[thick] (6.4, 3.5) -- (5.8, 3.5);
\draw[thick] (6.4, 3.2) rectangle (6.5, 4.2); 



\draw[path style] plot[domain=0:6.1, samples=50] (\x, {-0.25*(\x-4)^2 + 5});

\coordinate (P4) at (4, {-0.25*(4-4)^2 + 5});
\draw[dashed, gray!50] (P4) -- (P4 |- 0,0) node[above right, yshift=50pt] {$(x_4,y_4)$};
\draw (P4) node[above, point label style, ] {$t=4$};


\draw[vector style] (0,0) -- (P4);
\draw (2.5, 2.5) node[label style, text=obsidianGreen!70] {$\vec{r}_4$};



\def\angle{51.3} 
\draw[obsidianGreen!70, -] (1.5,0) arc (0:\angle:1.5);
\draw (\angle/2:1.7) node[label style, text=obsidianGreen!70, xshift=5pt] {$37^\circ$};

\foreach \t in {1, 2, ..., 5} {
    \pgfmathsetmacro{\yval}{-0.25*(\t-4)^2 + 5}
    \fill (\t, \yval) circle (1.5pt);
}

\end{tikzpicture}
\end{document}
```

$$
\begin{gather}
 \text{The ball's position, for example, could be identified to be:} \\ \\
(x_{4}\text{, }y_{4})\atop t=4 \\ \\
\text{Alternatively, the position vector specifies the distance and direction from the origin.} \\ \\
\vec{r_{4}} = (15\text{ m}, \text{ }37^{\circ})
\end{gather}
$$

---
#math #physics 
