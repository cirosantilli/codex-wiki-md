<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite horizon $N$, let $U_N[a,b]$ be the number of completed upcrossings by time $N$. Use the predictable strategy that holds one unit of the process after a visit below $a$ until the next visit above $b$. For a [supermartingale](../../../../../../supermartingale.md), the expected gain of this nonnegative predictable [martingale transform](../../../../../../martingale-transform.md) is nonpositive. Pathwise, the completed trades earn at least $(b-a)U_N[a,b]$, while an unfinished final trade can lose at most $(X_N-a)^-$. Hence

$$
(b-a)U_N[a,b]\leq (X_N-a)^-+(H\mathbin\cdot X)_N.
$$

Taking expectations and using $X_N\geq0$ gives the [Doob upcrossing inequality](../../../../../../doob-upcrossing-inequality.md)

$$
(b-a)\mathbb E U_N[a,b]
\leq\mathbb E(X_N-a)^-
\leq a.
$$

As $N\to\infty$, monotone convergence yields

$$
\boxed{\mathbb E U[a,b]\leq\frac a{b-a}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
