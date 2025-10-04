A tree-like data structure representing [[Source Code|source code]] in a hierarchical structure. [[Compiler (CS)|Compilers]] and [[Interpreter (CS)|interpreters]] utilize ASTs to analyze, optimize, and generate code. 

```tikz
\begin{document}
\begin{tikzpicture}[
  sibling distance=20mm,
  level distance=15mm,
  scale=1.5,
  yshift=-20cm,
  every node/.style={circle, draw, minimum size=7mm, inner sep=1mm, thick}
]
\node {+}
  child { node {a} }
  child { node {*}
    child { node {b} }
    child { node {c} }
  };
\end{tikzpicture}
\end{document}
```
<h4 font-size="12pt" align="center">AST Diagram</h4>

---
#computer-science 