The difference between the starting position of an object and its final position. Not to be confused with [[Distance|distance]], a [[Scalar|scalar]] quantity. It's drawn as a [[Vector Quantity|vector]] from its starting position to its final position.
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
      mark=at position 0.25 with {\arrow[obsidianPurple!70]{Stealth[length=6pt, width=6pt]}},
      mark=at position 0.5 with {\arrow[obsidianPurple!70]{Stealth[length=6pt, width=6pt]}},
      mark=at position 0.75 with {\arrow[obsidianPurple!70]{Stealth[length=6pt, width=6pt]}}
    }
  },
  displacement style/.style={obsidianGreen, ultra thick},
  point style/.style={fill=white, draw=black, circle, inner sep=1.5pt},
  label style/.style={font=\normalsize, text=obsidianGreen!70}
]

\draw[path style] (0,0) coordinate (start) .. controls +(1.5,2) and +(-1,-1.5) .. (4.3,0.5) coordinate (end);
\draw[displacement style] (start) -- (end) node[midway, below left, xshift=-10pt, yshift=-8, label style] {$\Delta r$};

\node[point style, gray!10, fill=gray!10, label={[obsidianPurple!70]below left:$r_i$}] at (start) {};
\node[point style, gray!10, fill=gray!10, label={[obsidianPurple!70]above right:$r_f$}] at (end) {};

\end{tikzpicture}
\end{document}
```
$$
\Delta r=r_{f}-r_{i}
$$
---

##### Displacement through [[Average Velocity|average velocity]]

You can solve for displacement by multiplying a given average velocity by the amount of time you'd like to attain the displacement for.
$$
\begin{gather} \\
\Delta x=\bar{v}\cdot t \\ \\
\end{gather}
$$
---

##### Getting the Kinematic Equation

When [[Acceleration|acceleration]] is [[constant]], the average velocity can be substituted for its equivalent [[Mathematical Expression|expression]] within the displacement [[equation]].
$$
\begin{gather} \\

\Delta x=\frac{1}{2}(v_i+v_{f})t \\

\end{gather}
$$

Suppose we do not have [[final velocity]]. In order to solve for displacement we may then substitute the final velocity for its equivalent expression:
$$
\begin{gather} \\

v_{f}=v_{i}+at \\ \\
\Delta x=\frac{1}{2}((v_{i}+v_{i}+at)\to (2v_{i}+at))t \\ \\
\Delta x=v_{i}t+\frac{1}{2}at^{2}
\end{gather}
$$
---
#physics 