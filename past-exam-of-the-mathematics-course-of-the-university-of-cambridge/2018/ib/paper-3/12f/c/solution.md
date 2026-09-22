<h1 id="12f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The closed bounded set $A\subset\mathbb R^m$ is [compact](../../../../../../compact-space.md) by the [Heine-Borel theorem](../../../../../../heine-borel-theorem.md). Choose a [convergent subsequence](../../../../../../convergent-subsequence.md) $x_{n_j}\to x_0$. For fixed $N$ and sufficiently large $j$, monotonicity gives

$$
g_N(x_{n_j})\geq g_{n_j}(x_{n_j})\geq\delta.
$$

Continuity and passage to the limit give $g_N(x_0)\geq\delta$ for every $N$, hence $\lim_Ng_N(x_0)\geq\delta$.

For the deduction, set $g_n=f_n-f$. These functions are continuous, decrease pointwise, and tend to zero. If convergence were not uniform, some $\delta>0$ would admit $x_n$ with $g_n(x_n)\geq\delta$. The result just proved would produce $x_0$ with $\lim g_n(x_0)\geq\delta$, contradicting pointwise convergence. Therefore **$f_n\to f$ uniformly**. This is [Dini's theorem](../../../../../../dini-s-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12F](../../12f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
