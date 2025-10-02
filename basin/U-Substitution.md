U-Substitution is a method used to clean up and solve seemingly messy integrals. You look to recognize an integrand with a specific pattern in order to simplify.
$$
\begin{gather}\\
f'(g(x))\cdot g'(x)
\end{gather}
$$
---
##### Workflow

1. Identify $\large{u}$. Typically identified by being the argument of a trig function, inside a parentheses, under a square root, or inside an exponent.
:
2. Differentiate $\large{u}$ with respect to the variable in the function, and then solve for $\large{du}$.
:
3. Rewrite the entire integral in terms of $\large{u}$, replacing the `inside expression` with $\large{u}$ and the `outside expression` (alongside $\large{dx}$) with $\large{du}$.
:
4. Integrate the now simpler integral with respect to $\large{u}$ using [[Integration Rules|integration rules]].
:
5. Back-substitute $\large{u}$ and finish simplifying.

---
##### Example
$$
\begin{gather} \\
\int \sin ^{3}(x)\cos(x)\ dx \\ \\
\int(\sin(x))^{3}\cos(x)\ dx \\ \\
u=\sin(x) \\ \\
\frac{du}{dx}=\cos(x) \\ \\
du=\cos(x)\ dx \\ \\
\int(u)^{3}du \\ \\
\frac{u^{4}}{4} +C \\
\frac{1}{4}\cdot(\sin(x))^{4}+C\to \frac{\sin ^{4}(x)}{4}+C
\end{gather}
$$

---
#math #calculus 