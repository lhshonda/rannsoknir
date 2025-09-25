2025-09-25 // 15:18

:: [[Mathematics]]

---

Two specific types of [[Right Angle|right triangles]] with predictable side-length ratios. Knowing a single side allows us to determine all of the other missing side lengths!

---

>45-45-90 Triangle - Isosceles Right Triangle

The angles will always be $45^\circ$, $45^\circ$, and $90^\circ$. The two legs are always equal in length, while the hypotenuse is $\sqrt{ 2 }$ times the length of a leg: i.e., if a leg opposite a $45^\circ$ angle is $x$, the ratio of the triangle is $x:x:x\sqrt{ 2 }$.


```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}

\begin{tikzpicture}[
  scale=2,
  line style/.style={thick},
  label style/.style={font=\small},
  angle style/.style={font=\small, text=obsidianPurple},
  right angle style/.style={draw, thick}
]


\coordinate (A) at (0,0);
\coordinate (B) at (2,0);
\coordinate (C) at (0,2);


\draw[line style] (A) -- (B) node[midway, below, label style] {$x$};
\draw[line style] (A) -- (C) node[midway, left, label style] {$x$};
\draw[line style] (B) -- (C) node[midway, above right, label style] {$x\sqrt{2}$};


\draw[right angle style] (A) ++(0,0.2) -- ++(0.2,0) -- ++(0,-0.2);



\draw[obsidianPurple, -] (B) +(180:0.5) arc (180:135:0.5);
\draw (B) + (157.5:0.65) node[angle style] {$45^\circ$};


\draw[obsidianPurple, -] (C) +(-90:0.5) arc (-90:-45:0.5);
\draw (C) + (-67.5:0.65) node[angle style] {$45^\circ$};

\end{tikzpicture}
\end{document}
```


---

>30-60-90 Triangle

With the angles of $30^\circ$, $60^\circ$, and $90^\circ$. The hypotenuse is twice the length of the shortest leg, while the longer leg is $\sqrt{ 3 }$ times the shortest one. 


```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}

\begin{tikzpicture}[
  scale=3,
  line style/.style={thick},
  label style/.style={font=\small},
  angle style/.style={font=\small, text=obsidianPurple},
  right angle style/.style={draw, thick}
]

\coordinate (A) at (0,0);
\coordinate (B) at ({sqrt(3)},0);
\coordinate (C) at (0,1);          


\draw[line style] (A) -- (B) node[midway, below, label style] {$x\sqrt{3}$};
\draw[line style] (A) -- (C) node[midway, left, label style] {$x$};
\draw[line style] (B) -- (C) node[midway, above right, label style] {$2x$};


\draw[right angle style] (A) ++(0,0.2) -- ++(0.2,0) -- ++(0,-0.2);


\def\angleB{30}
\draw[obsidianPurple, -] (B) +(180:0.5) arc (180:{180-\angleB}:0.5);
\draw (B) + (165:0.65) node[angle style] {$30^\circ$};


\def\angleC{60}
\draw[obsidianPurple, -] (C) +(-90:0.5) arc (-90:{-90+\angleC}:0.5);
\draw (C) + (-60:0.65) node[angle style] {$60^\circ$};

\end{tikzpicture}
\end{document}
```

---

