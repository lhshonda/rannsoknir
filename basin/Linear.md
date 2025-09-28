2025-09-09 // 19:10

:: [[Mathematics]]

---

Linearity, the state/property of being linear within mathematics, is defined by the direct and proportional relationship between variables. For a function to be linear it's output must change in proportion to the change in input. 

>The slope, i.e. its rise over run, must be [[constant]]!

```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\definecolor{obsidianGreen}{rgb}{0.455,0.639,0.036}

\begin{tikzpicture}[
  scale=1.5,
  every node/.style={font=\small},
  axis style/.style={->, gray!70, thick},
  line style/.style={thick, obsidianPurple},
  label style/.style={font=\large}
]


\draw[axis style] (-1,0) -- (4,0) node[right] {$x$};
\draw[axis style] (0,-1) -- (0,3) node[above] {$y$};



\def\slopeValue{0.5}
\draw[line style] (-0.8, {-0.8 * \slopeValue}) -- (3.8, {3.8 * \slopeValue});


\draw (3.5, {3.5 * \slopeValue}) node at (3.5,1.6) [right, label style, obsidianPurple!70] {$y = mx$};


\draw[dashed, gray!50] (1,0) -- (1, {1 * \slopeValue}) -- (0, {1 * \slopeValue});
\draw (1, {1 * \slopeValue}) node at (0.6,0.7) [obsidianPurple!70] {$(x_1, y_1)$};
\fill[obsidianPurple!70] (1, {1 * \slopeValue}) circle (1.5pt);

\draw[dashed, gray!50] (2.5,0) -- (2.5, {2.5 * \slopeValue}) -- (0, {2.5 * \slopeValue});
\draw (2.5, {2.5 * \slopeValue}) node at (2.15,1.45) [obsidianPurple!70] {$(x_2, y_2)$};
\fill[obsidianPurple!70] (2.5, {2.5 * \slopeValue}) circle (1.5pt);


\def\constantC{2.5} 
\draw[thick, obsidianGreen] (-0.8, \constantC) -- (3.8, \constantC);
\draw (3.5, \constantC) node[below, xshift=-30pt, label style, obsidianGreen!70] {$y = b$}; 
\fill[obsidianGreen!70] (0, \constantC) circle (1.5pt); 

\end{tikzpicture}
\end{document}
```
$$
\begin{gather}
\text{Though it might seem counterintuive, a constant function is also linear.} \\
\text{To never change is still a state of constant change. } \\
\text{Just constantly unchanging.}
\end{gather}
$$
---
