2025-09-16 // 19:59

:: [[Mathematics]]

---

These are some of the useful environments to keep in mind in order to take nice mathematical notes with $\LaTeX$, in combination with the plugin I use on obsidian.

I will typically initiate a centered math aware block with the keyword `dm`, and follow up with `beg` in order to articulate my specific env. 

```
$$
begin{}

end{}
$$
```

The cursor is automatically placed in between both delimiters. I typically then use `gather` in order to center multiple equations on separate lines. As you *return* each line, `\\` are automatically entered to denote the line break.

---

> I found a lot of these environments through trial and error. I specifically pull this one from amsmath, a $\LaTeX$ package typically included with `\usepackage{amsmath}`. The statement was unnecessary within my notes though, and I am unsure why. Take all knowledge obtained from this writeup with a grain of salt. My understand of how $LaTeX$ Suite behaves is incomplete.

---

The following block:

```
$$
begin{gather}
2x+5 \\
\text{This can be referred to as an expression.}
end{gather}
$$
```

Results into:

$$
\begin{gather}
2x+5 \\
\text{This can be referred to as an expression.}
\end{gather}
$$

> `\text{}` is inputted with the respective key bind and keyword: `"` and `text`.
> Any further shortcuts may be found or configured within the $LaTeX$ Suite plugin.

---
