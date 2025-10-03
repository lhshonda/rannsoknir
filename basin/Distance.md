In physics, **distance** refers to the [[Magnitude (Physics)|magnitude]], i.e. the total length of the path an object travels. Being a [[Scalar|scalar]] quantity, it does not account for direction in the same way [[Displacement|displacement]] does. 

>An object's total path, distance, can never be negative. Its lowest value will always be zero in the event the object never moves.

```tikz
\begin{document}

\usetikzlibrary{decorations.markings,arrows.meta}
\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}
\definecolor{obsidianGreen}{rgb}{0.455,0.639,0.036}

\begin{tikzpicture}[
  scale=1.5,
  every node/.style={font=\small},
  path style/.style={
    obsidianPurple, very thick,
    postaction={decorate},
    decoration={
      markings,
      mark=at position 0.3 with {\arrow[obsidianPurple!70]{Stealth[length=3pt, width=3pt]}},
      mark=at position 0.6 with {\arrow[obsidianPurple!70]{Stealth[length=3pt, width=3pt]}}
    }
  },
  displacement style/.style={obsidianGreen, thick, dashed},
  point style/.style={fill=white, draw=black, circle, inner sep=1.5pt},
  label style/.style={font=\normalsize}
]


\draw[path style] (0,0) coordinate (start) .. controls +(1.5,2) and +(-1,-1.5) .. (4.3,0.5) coordinate (end);
\draw[displacement style] (start) -- (end);


\draw (0.7, 1.05) node[label style, text=obsidianPurple!70] {Distance};
\draw (2.15, -0.2) node[label style, text=obsidianGreen!70] {Displacement};


\node[point style, gray!10, fill=gray!10, label={below left:Start}] at (start) {};
\node[point style, gray!10, fill=gray!10, label={above right:End}] at (end) {};

\end{tikzpicture}
\end{document}
```
---
#physics 