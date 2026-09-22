<h1 id="12e/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $(x_n)$ be a [Cauchy sequence](../../../../../../../cauchy-sequence.md) in a compact metric space $X$. By [sequential compactness of a compact metric space](../../../../../../../sequential-compactness-of-a-compact-metric-space.md), it has a [convergent subsequence](../../../../../../../convergent-subsequence.md) $x_{n_j}\to x\in X$. Given $\varepsilon>0$, choose $N$ such that $d(x_m,x_n)<\varepsilon/2$ whenever $m,n\geq N$, and then choose $j$ such that $n_j\geq N$ and $d(x_{n_j},x)<\varepsilon/2$. For every $n\geq N$, the [triangle inequality](../../../../../../../triangle-inequality.md) gives

$$
d(x_n,x)\leq d(x_n,x_{n_j})+d(x_{n_j},x)<\varepsilon.
$$

**Thus the whole sequence converges to $x$. Every Cauchy sequence converges in $X$, so $X$ is a [complete metric space](../../../../../../../complete-metric-space.md).**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [12E](../../../12e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
