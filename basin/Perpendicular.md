2025*-09-24 // 23:05

:: [[Mathematics]]

---

Defined by an intersection of two objects at a [[Right Angle|right angle]]. 
Perpendicularity may be represented by $\perp$.

```tikz
\begin{document}
\begin{tikzpicture}[scale=1.2, font=\small]

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}


\draw [<->] (-3,0) -- (4,0) node[below left] {$x$};
\draw [<->] (0,-2) -- (0,4) node[below left] {$y$};



\draw[obsidianPurple, thick, dashed] (-3,-1) -- (3,2);


\draw[obsidianPurple, thick, dashed] (0,3) -- (2,-1);

\begin{scope}[shift={(1,1)}, rotate=26.57]
    \draw[red!40, blue!40, thick] (0.25,0) -- (0.25,0.25) -- (0,0.25);
\end{scope}


\node[align=center, fill=white, inner sep=2pt] at (2.5,-1.5) {Perpendicular Lines \\ $L_1 \perp L_2$ \\ $m_1 \cdot m_2 = -1$};

\end{tikzpicture}
\end{document}
```


> The slope of two perpendicular slopes equal $-1$ when multiplied.

---

