<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix distinct players $i,j$ and write $Ti=T\cup\{i\}$, with analogous notation for $Tj$ and $Tij$. Splitting sampled [coalitions](../../../../../coalition-game-theory.md) according to whether they contain the other player gives

$$
\begin{aligned}
2^{n-1}\beta_i(v)&=\sum_{T\subseteq N\setminus\{i,j\}}\bigl[v(Ti)-v(T)+v(Tij)-v(Tj)\bigr],\\
2^{n-1}\beta_j(v)&=\sum_{T\subseteq N\setminus\{i,j\}}\bigl[v(Tj)-v(T)+v(Tij)-v(Ti)\bigr].
\end{aligned}
$$

Subtracting yields the [Banzhaf difference identity](../../../../../banzhaf-difference-identity.md),

$$
\beta_j(v)-\beta_i(v)=\frac1{2^{n-2}}\sum_{T\subseteq N\setminus\{i,j\}}\bigl[v(Tj)-v(Ti)\bigr].
$$

In a [weighted voting game](../../../../../weighted-voting-game.md), $w_j>w_i$ means that $Tj$ has greater total weight than $Ti$. Thus $v(Tj)\geq v(Ti)$ for every $T$: if the lighter [coalition](../../../../../coalition-game-theory.md) reaches the quota, the heavier one does too. Every summand is nonnegative, proving **$\beta_i(v)\leq\beta_j(v)$**. Equality remains possible even when the weights differ.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
