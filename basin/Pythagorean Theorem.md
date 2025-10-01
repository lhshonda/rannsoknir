The pythagorean theorem is a fundamental relation in [[Euclidean Geometry|Euclidean geometry]] between the sides of a [[Right Angle|right]] triangle. It states that in any right angled triangle, the square of the hypotenuse is equal to the sum of the squares of the other two sides. 

>The trigonometric identity, $\sin ^{2}(\theta)+\cos ^{2}(\theta)=1$, is Pythagoras' theorem in disguise!


```tikz
\begin{document}

\definecolor{obsidianPurple}{rgb}{0.545,0.361,0.964}

\begin{tikzpicture}[
  scale=2,
  line style/.style={thick},
  label style/.style={font=\large},
  right angle style/.style={draw, thick}
]


\coordinate (A) at (0,0);
\coordinate (B) at (3,0);
\coordinate (C) at (0,2);


\draw[line style] (A) -- (B) node[midway, below, label style] {$b$};
\draw[line style] (A) -- (C) node[midway, left, label style] {$a$};
\draw[line style] (B) -- (C) node[midway, above right, label style] {$c$};


\draw[right angle style, obsidianPurple] (A) ++(0,0.2) -- ++(0.2,0) -- ++(0,-0.2);

\node[label style, obsidianPurple] at (0.4,0.3) {$90^\circ$};


\draw (1.5, -0.7) node[label style, text=gray!10] {$a^2 + b^2 = c^2$};

\end{tikzpicture}
\end{document}
```

---
#math