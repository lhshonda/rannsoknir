2025-09-24 // 23:07

:: [[Mathematics]]

---

An angle of $90^\circ$ or $\frac{\pi}{2}$ radians. 
Commonly created by the perpendicular intersection of two elements.

```tikz
\begin{document}

\begin{tikzpicture}[scale=0.8]

% Draw the positive x and y axes with arrows
\draw [->, thick] (0,0) -- (5,0) node[anchor=north east] {$x$};
\draw [->, thick] (0,0) -- (0,5) node[anchor=south west] {$y$};

% Draw the square symbol for the 90-degree angle
\draw (0.4,0) -- (0.4,0.4) -- (0,0.4);

% Add the 90-degree text label
\node at (0.8,0.8) {$90^\circ$};

\end{tikzpicture}

\end{document}
```