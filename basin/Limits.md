2025-09-16 // 18:42

:: [[Mathematics]]

---

The value approached as an argument approaches some value.

$$
\begin{gather}
\lim_{ x \to \text{ a} } f(x) = L  \\ \\

\text{As } x \text{ gets close to } a\text{, }f(x)\text{ gets close to }L\text{.}
\end{gather}
$$

> When taking the limit of expressions, by definition, we implicitly treat said expression as a defined function of an argument. It's done so for the sake and context of the limit process itself, not as an assertion of an equation, or a full invocation of all properties of [[Function|functions]].

--- 

The direction of approach is dictated by a positive/negative superscript on the argument. When calculating two sided limits, the value approached from both direction must be the same.

$\displaystyle \lim_{ x \to \text{ a}^{+} }f(x) \text{ approaches a from the right.}$
$\displaystyle\lim_{ x \to \text{ a}^{-} }f(x) \text{ approaches a from the left.}$

Here, $a$ is the argument and the $\pm$ constitutes the direction of approach.

---

In the event passing an argument into an expression directly outputs a real number within its domain, then you may consider the output the limit itself. This does not constitute a function's output as the limit, but instead allows for its output to be observed as the value approached for the argument. 

>*Discontinuous functions may still contain two-sided limits at said discontinuous points.*

$$
\begin{gather}
\lim_{ x \to 1 } f\left(x\right)=\frac{x^{2}-1}{x-1} \\
\text{As }x\text{ approaches }1\text{ the limit is 2 yet the function is} \\
\text{undefined at that point.}
\end{gather}
$$

When solving limits, you may pass in an argument and an expression may result in an something such as an [[Indeterminate Form|indeterminate form]]. Said limits determined with methods such as [[L'Hôpital's Rule|L'Hôpital's rule]] or by simply graphing the function if allowed. 

$$
\begin{gather}
\lim_{ x \to 1 } \frac{1}{x}=\frac{1}{0} \\
\end{gather}
$$

```tikz
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[very thin,color=gray] (-0.1,-1.1) grid (3.9,3.9);
    \draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$};
    \draw[->] (0,-1.2) -- (0,4.2) node[above] {$f(x)$};
    \draw[color=red]    plot (\x,\x)             node[right] {$f(x) =x$};
    \draw[color=blue]   plot (\x,{sin(\x r)})    node[right] {$f(x) = \sin x$};
    \draw[color=orange] plot (\x,{0.05*exp(\x)}) node[right] {$f(x) = \frac{1}{20} \mathrm e^x$};
  \end{tikzpicture}
\end{document}
```

```
\begin{document}
  \begin{tikzpicture}[domain=0:4]
    \draw[very thin,color=gray] (-0.1,-1.1) grid (3.9,3.9);
    \draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$};
    \draw[->] (0,-1.2) -- (0,4.2) node[above] {$f(x)$};
    \draw[color=red]    plot (\x,\x)             node[right] {$f(x) =x$};
    \draw[color=blue]   plot (\x,{sin(\x r)})    node[right] {$f(x) = \sin x$};
    \draw[color=orange] plot (\x,{0.05*exp(\x)}) node[right] {$f(x) = \frac{1}{20} \mathrm e^x$};
  \end{tikzpicture}
\end{document}
```

```tik
\begin{document}
 \begin{tikzpicture}[domain=-5:5]
    \\draw[very thin,color=gray] (-5.1,-5.1) grid (5.1,5.1);
    \\draw[->] (-5.2,0) -- (5.2,0) node[right] {$x$};
    \\draw[->] (0,-5.2) -- (0,5.2) node[above] {$f(x)$};
    \\draw[blue,thick,domain=-5:5,samples=400] plot (\\x,{<++>});
  \\end{tikzpicture}
\\end{document}
```

```
"```tikz\n\\begin{document}\n  \\begin{tikzpicture}[domain=-5:5]\n    \\draw[very thin,color=gray] (-5.1,-5.1) grid (5.1,5.1);\n    \\\\draw[->] (-5.2,0) -- (5.2,0) node[right] {$x$};\n    \\\\draw[->] (0,-5.2) -- (0,5.2) node[above] {$f(x)$};\n    \\\\draw[blue,thick,domain=-5:5,samples=400] plot (\\\\x,{<++>});\n  \\\\end{tikzpicture}\n\\\\end{document}\n```",
```

```
"```tikz"
\begin{document}
\begin{tikzpicture}[domain=0:4]
  \draw[very thin,color=gray] (-0.1,-1.1) grid (8,3.9);

  \draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$};
  \draw[->] (0,-1.2) -- (0,4.2) node[above] {$f(x)$};

  \draw[color=red]    plot (\x,\x)             node[right] {$f(x) =x$};
  % \x r means to convert '\x' from degrees to _r_adians:
  \draw[color=blue]   plot (\x,{sin(\x r)})    node[right] {$f(x) = \sin x$};
  \draw[color=orange] plot (\x,{0.05*exp(\x)}) node[right] {$f(x) = \frac{1}{20} \mathrm e^x$};
\end{tikzpicture}
\end{document}
"```"
```

```tikz
\begin{document}
\begin{tikzpicture}[domain=-4:4]
  \draw[very thin,color=black] (-0.1,-1.1) grid (-3.9,4);

  \draw[->] (-0.2,0) -- (4.2,0) node[right] {$x$};
  \draw[->] (0,-1.2) -- (0,4.2) node[above] {$f(x)$};

  \draw[color=red]    plot (\x,\x)             node[right] {$f(x) =x$};
  % \x r means to convert '\x' from degrees to _r_adians:
  \draw[color=blue]   plot (\x,{sin(\x r)})    node[right] {$f(x) = \sin x$};
  \draw[color=orange] plot (\x,{0.05*exp(\x)}) node[right] {$f(x) = \frac{1}{20} \mathrm e^x$};
\end{tikzpicture}
\end{document}
```
```tikz
\begin{document}
\usetikzlibrary {datavisualization.formats.functions}
\tikz \datavisualization [scientific axes=clean, scale=1]
[
  visualize as smooth line=Gaussian,
  Gaussian={pin in data={text={$e^{-x^2}$},when=x is 1}}
]
data [format=function] {
  var x : interval [-7:7] samples 51;
  func y = exp(-\value x*\value x);
}
[
  visualize as scatter,
  legend={south east outside},
  scatter={
    style={mark=*,mark size=1.4pt},
    label in legend={text={
        $\sum_{i=1}^{10} x_i$, where $x_i \sim U(-1,1) $}}}
]
data [format=function] {
  var i : interval [0:1] samples 20;
  func y = 0;
  func x = (rand + rand + rand + rand + rand +
rand + rand + rand + rand + rand);
};
\end{document}
```
```
begin{document}

end{document}
```

```
\usetikzlibrary {datavisualization}
\begin{tikzpicture}
  \datavisualization [school book axes, visualize as line]
    data [format=named] {
      x=0, y=0
      x=1, y=1
      x=2, y=1
      x=3, y=0
    };
\end{tikzpicture}
```

```tikz
\begin{document}
\usetikzlibrary {datavisualization}
\begin{tikzpicture}
  \datavisualization [school book axes, visualize as line]
    data [format=named] {
      x=0, y=0
      x=1, y=1
      x=2, y=1
      x=3, y=0
    };
\end{tikzpicture}
\end{document}
```




```tikz
\begin{document}
\usetikzlibrary {datavisualization.formats.functions}
\begin{tikzpicture} \datavisualization [
  school book axes,
  all axes={unit length=5mm, ticks={step=2}},
  visualize as smooth line]
data [format=function] {
  var t : interval [0:2*pi];

  func x = \value t * cos(\value t r);
  func y = \value t * sin(\value t r);
};
\end{tikzpicture}
\end{document}
```




 
> Petri-net diagrams look and are made through the custom snippets provided in [[Figure 1.2]]:

```tikz
\begin{document}
\usetikzlibrary {petri}
\begin{tikzpicture}[yscale=-1.6,xscale=1.5,thick,
  every transition/.style={draw=red,fill=red!20,minimum size=3mm},
  every place/.style={draw=blue,fill=blue!20,minimum size=6mm}]

  \foreach \i in {1,...,6} {
    \node[place,label=left:$p_\i$] (p\i) at (0,\i) {};
    \node[place,label=right:$q_\i$] (q\i) at (8,\i) {};
  }
  \foreach \name/\var/\vala/\valb/\height/\x in
      {m1/m_1/f/t/2.25/3,m2/m_2/f/t/2.25/5,h/\mathit{hold}/1/2/4.5/4} {
    \node[place,label=above:{$\var = \vala$}] (\name\vala) at (\x,\height) {};
    \node[place,yshift=-8mm,label=below:{$\var = \valb$}] (\name\valb) at (\x,\height) {};
  }
  \node[token] at (p1) {};   \node[token] at (q1) {};
  \node[token] at (m1f) {};  \node[token] at (m2f) {};
  \node[token] at (h1) {};

  \node[transition] at (1.5,1.5) {}  edge [pre] (p1)  edge [post] (p2);
  \node[transition] at (1.5,2.5) {}  edge [pre] (p2)  edge[pre]   (m1f)
                                     edge [post](p3)  edge[post]  (m1t);
  \node[transition] at (1.5,3.3) {}  edge [pre] (p3)  edge [post] (p4)
                                     edge [pre and post] (h1);
  \node[transition] at (1.5,3.7) {}  edge [pre] (p3)  edge [pre] (h2)
                                     edge [post] (p4) edge [post] (h1.west);
  \node[transition] at (1.5,4.3) {}  edge [pre] (p4)  edge [post] (p5)
                                     edge [pre and post] (m2f);
  \node[transition] at (1.5,4.7) {}  edge [pre] (p4)  edge [post] (p5)
                                     edge [pre and post] (h2);
  \node[transition] at (1.5,5.5) {}  edge [pre] (p5)  edge [pre] (m1t)
                                     edge [post] (p6) edge [post] (m1f);
  \node[transition] at (1.5,6.5) {}  edge [pre] (p6)  edge [post] (p1.south east);
  \node[transition] at (6.5,1.5) {}  edge [pre] (q1)  edge [post] (q2);
  \node[transition] at (6.5,2.5) {}  edge [pre] (q2)  edge [pre] (m2f)
                                     edge [post] (q3) edge [post] (m2t);
  \node[transition] at (6.5,3.3) {}  edge [pre] (q3)  edge [post] (q4)
                                     edge [pre and post] (h2);
  \node[transition] at (6.5,3.7) {}  edge [pre] (q3)  edge [pre] (h1)
                                     edge [post] (q4) edge [post] (h2.east);
  \node[transition] at (6.5,4.3) {}  edge [pre] (q4)  edge [post] (q5)
                                     edge [pre and post] (m1f);
  \node[transition] at (6.5,4.7) {}  edge [pre] (q4)  edge [post] (q5)
                                     edge [pre and post] (h1);
  \node[transition] at (6.5,5.5) {}  edge [pre] (q5)  edge [pre] (m2t)
                                     edge [post] (q6) edge [post] (m2f);
  \node[transition] at (6.5,6.5) {}  edge [pre] (q6)  edge [post] (q1.south west);
\end{tikzpicture}
\end{document}
```




$$
\begin{gather} \\


\end{gather} \\

$$
```tikz
\begin{document}
\begin{tikzpicture}
\usetikzlibrary {datavisualization.formats.functions}
\datavisualization [scientific axes=clean]
[
  visualize as smooth line=Gaussian,
  Gaussian={pin in data={text={$e^{-x^2}$},when=x is 1}}
]
data [format=function] {
  var x : interval [-7:7] samples 51;
  func y = exp(-\value x*\value x);
}
[
  visualize as scatter,
  legend={south east outside},
  scatter={
    style={mark=*,mark size=1.4pt}}
]
data [format=function] {
  var i : interval [0:1] samples 20;
  func y = 0;
  func x = (rand + rand + rand + rand + rand +
rand + rand + rand + rand + rand);
};
\end{tikzpicture}
\end{document}
```




```tikz
\begin{document}
\begin{tikzpicture}
\usetikzlibrary {datavisualization.formats.functions}
  \datavisualization [school book axes, visualize as smooth line,
    x axis={ticks={minor steps between steps}},
    y axis={ticks={minor steps between steps}},
  ]
    data [format=function] {
      var x : interval [-1.5:1.5];
      func y = \value x^2;
    };
\end{tikzpicture}
\end{document}
```

```tikz
\begin{document}
\begin{tikzpicture}
\usetikzlibrary {datavisualization.formats.functions}
  \datavisualization [school book axes, visualize as smooth line,
    x axis={ticks={minor steps between steps=3}},

  ]
    data [format=function] {
      var x : interval [-1.5:1.5];
      func y = (\value x)^2;
    };
\end{tikzpicture}
\end{document}
```

```tikz

\usepackage{pgfplots}
\pgfplotsset{compat=1.16}


\begin{document}
%Here begins the 2D plot
\begin{tikzpicture}
\begin{axis}
\addplot[color=red]{exp(x)};
\end{axis}
\end{tikzpicture}
%Here ends the 2D plot
\hskip 5pt
%Here begins the 3D plot
\begin{tikzpicture}
\begin{axis}[colormap/viridis]
\addplot3[
    surf,
    samples=18,
]
{exp(-x^2-y^2)*x};
\end{axis}
\end{tikzpicture}
%Here ends the 3D plot
\end{document}
```
```tikz
\usepackage{pgfplots}
\pgfplotsset{compat=1.16}

\begin{document}

\begin{tikzpicture}
\begin{axis}[colormap/viridis]
\addplot3[
	surf,
	y domain=-2:2,
	samples=18,
	domain=-3:3
]
{exp(-x^2-y^2)*x};
\end{axis}
\end{tikzpicture}

\end{document}
```

```tikz
\usepackage{pgfplots}
\pgfplotsset{compat=1.16}
\begin{document}
\begin{tikzpicture}
\begin{axis}[colormap/viridis]
\addplot3[
    surf,
    shader=flat,
    samples=25,
    domain=-2:2,
    mesh/ordering=x varies,
	restrict z to domain=-1e6:1e6
]
{exp(-x^2-y^2)*x};
\end{axis}
\end{tikzpicture}
%Here ends the 3D plot
\end{document}
```