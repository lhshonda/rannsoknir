2025-09-25 // 00:43

:: [[Mathematics]]

---

Pi, symbolically represented by π, is a [[Mathematical Constant|mathematical constant]] defined as the ratio of a circle's [[Circumference|circumference]] to its [[Diameter|diameter]]. Since π is an [[Irrational Number|irrational number]], it cannot be represented by the ratio of two integers. It goes on forever without falling into a repeating pattern.

$$
\begin{gather}
\pi = \frac{\text{Circumference}}{\text{Diameter}}=\frac{C}{d} \\
 \\
\pi d=C\\
2\pi r=C
\end{gather}
$$

> The definition of π holds true for every circle in the universe.

```tikz
\begin{document}

\usetikzlibrary{decorations.pathreplacing}

\begin{tikzpicture}[
  scale=1.1,
  every node/.style={text=white}
]

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}


\def\r{1.5}
\def\d{3}
\coordinate (C) at (-1, 2.5);


\draw[thick] (C) circle (\r);


\draw[-, dashed] (-1-\r, 2.5) -- (-1+\r, 2.5);
\draw (-1, 2.5) node[below=4pt, text=cyan] {Diameter, $d$};


\def\circ{3.1416 * \d}
\coordinate (start) at (0, 0);
\draw[-, thick, dashed] (start) --++ (\circ, 0);
\draw (start) node[below left] {$0$};
\draw (\circ, 0) node[below right] {Circumference, $C$};


\draw[thick, obsidianPurple] (0, 0) arc (180:0:\d/2);
\draw (\d/2, 0) node[above, text=yellow] {$d$};

\draw[thick, obsidianPurple] (\d, 0) arc (180:0:\d/2);
\draw (\d + \d/2, 0) node[above, text=magenta] {$d$};

\draw[thick, obsidianPurple] (2*\d, 0) arc (180:0:\d/2);
\draw (2*\d + \d/2, 0) node[above, text=cyan] {$d$};


\def\rem{\circ - 3*\d}
\draw[decoration={brace,amplitude=4pt},decorate,thick, red!20, blue!20] (3*\d, 0.2) -- (3*\d + \rem, 0.2) node[right, text=red!20, blue!20] {$\approx 0.14d$};



\draw (6, 3) node[text=yellow, align=center, font=\large] {$\pi = \frac{C}{d} \approx 3.14159$};

\end{tikzpicture}
\end{document}
```



