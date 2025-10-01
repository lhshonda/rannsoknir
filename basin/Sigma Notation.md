Also know as summation notation within mathematics, sigma notation represents [[Summation|summation]] through the Greek capital letter sigma $\Sigma$. Though $i$ is used to represent the index of summation, other common ones include: $j$, $k$, and $n$.

$$
\begin{gather}
\sum_{i=1}^{n}a_{i} \\ \\
\text{The sum of }a_{i}\text{ from }i=1\text{ to }i=n. \\
a_{i}\text{ representing the rule for all terms added.}
\end{gather}
$$

---

>Sigma Notation Properties

The **constant multiple rule** allows for [[Constant|constants]] to be factored out. This essentially is the [[Distributive Property|distributive property]] applied in summation.

$$
\begin{gather}
\sum_{i=1}^{n}c\cdot a_{i}=c\cdot \sum_{i=1}^{n} a_{i}
\end{gather}
$$

The **sum and difference rule** states the sum of two [[Mathematical Expression|expressions]] is the same as their individual sums.

$$
\begin{gather}
\sum_{i=1}^{n} (a_{i}\pm b_{i})=\sum_{i=1}^{n} a_{i}\pm \sum_{i=1}^{n} b_{i}
\end{gather}
$$

**Summing a constant** a certain amount is the same as the [[Product|product]] of the constant and the amount of times it's summed over.

$$
\begin{gather}
\sum_{i=1}^{n} c=c\cdot n
\end{gather}
$$

The **associative property**, or the rule for **splitting a sum** allows for a larger sum to be split into two smaller consecutive sums.

$$
\begin{gather}
\sum_{i=1}^{n} a_{i}=\sum_{i=1}^{m}a_{i}+\sum_{i=m+1}^{n} a_{i} \\ \\
\end{gather}
$$

>When using these properties, you may separate the sum of an integer, and it may seem somewhat confusing. We may expect the summation rule to contain a variable such as $i$, but a constant rule is perfectly valid.

$$
\begin{gather} \\
\sum_{i=1}^{20} 1=20 \\ \\
\text{\textbf{The summation above asks:}} \\
\text{From }i=1\text{ to }i=20\text{ what does the ``rule'' of the sum generate?} \\ \\
\text{The rule in this case is simply a constant function equal to 1.} \\ \\
\end{gather} 
$$
---

>Writing a series in **Sigma Notation**

$$
\begin{gather}
3+6+9+12+15 \\ \\
\text{Identify the pattern.} \\
\text{Here we have each term as a multiple of 3.} \\
\text{The function }3i\text{ represents the }i\text{-th term.} \\
\text{The last term, }15\text{, is represented by the final index n.} \\ \\

\sum_{i=1}^{5} 3i
\end{gather}
$$

---
#math #calculus 
