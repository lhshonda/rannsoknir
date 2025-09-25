2025-09-24 // 23:05

:: [[Mathematics]]

---

Defined by an intersection of two objects at a [[Right Angle|right angle]]. 
Perpendicularity may be represented by the symbol: $\perp$

```tikz
\begin{document}
\begin{tikzpicture}[scale=1.2, font=\small]

% --- Axes ---
\draw [<->] (-3,0) -- (4,0) node[below left] {$x$};
\draw [<->] (0,-2) -- (0,4) node[below left] {$y$};

% --- Lines ---
% L1 with slope m = 1/2. Equation: y = 0.5x + 0.5
\draw[yellow] (-3,-1) -- (3,2);

% L2 with slope m = -2. Equation: y = -2x + 3
\draw[red] (0,3) -- (2,-1);

% --- Angle & Labels ---
% The lines intersect at (1,1). We'll place the right-angle symbol there.
% The angle of L1 is atan(0.5) which is approx 26.57 degrees. We rotate our square by that much.
\begin{scope}[shift={(1,1)}, rotate=26.57]
    \draw[gray, thick] (0.25,0) -- (0.25,0.25) -- (0,0.25);
\end{scope}

% Add a descriptive label for the concept
\node[align=center, fill=white, inner sep=2pt] at (2.5,-1.5) {Perpendicular Lines \\ $L_1 \perp L_2$ \\ $m_1 \cdot m_2 = -1$};

\end{tikzpicture}
\end{document}
```


> The slope of two perpendicular slopes equal $-1$ when multiplied.

