Unit used for measuring angles. Defined by the radius of a circle–a radian is measured by the angle created when the length of the radius is wrapped around the edge of a circle.


```tikz
\begin{document}
\begin{tikzpicture}[
  scale=1.3,
  font=\small,
  angle_label/.style={color=cyan},
  radius_label/.style={color=cyan},
  arc_label/.style={color=cyan}
]


\def\myradius{2.5}
\def\radianangle{57.2958}


\draw[gray, dashed] (0,0) circle (\myradius);


\draw[thick] (0,0) -- (\myradius,0) node[midway, below=2pt, radius_label] {Radius ($r$)};


\draw[thick] (0,0) -- (\radianangle:\myradius);


\draw[very thick] (\myradius,0) arc (0:\radianangle:\myradius) node[midway, right, arc_label] {Arc length = $r$};


\draw[->] (1,0) arc (0:\radianangle:1) node[midway, right=3pt, angle_label] {1 radian};


\fill (0,0) circle (1.5pt);

\end{tikzpicture}
\end{document}
```


> Since the radian is based on a **proportion**, not a fixed length, it will always be defined by the same angle of $57.2958^\circ$.

If you double the radius of a circle, you end up doubling the length of the arc needed to make a radian, thus keeping the angle identical. 

---

A circle's [[Circumference|circumference]] is defined as $2\pi r$. Following this logic, it takes $2\pi$ radius-lengths to go around the entirety of the circle.

$$
\begin{gather}
180^\circ=\pi \text{ radians.} \\
 \\
\text{Half of 2}\pi\text{ is }\pi\text{. }\\
\text{Thus }\pi\text{ radians is 180}^\circ \text{ since a full circle is 360}^\circ.
\end{gather}
$$

---
#math 