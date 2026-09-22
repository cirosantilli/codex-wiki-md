<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By the [Tonelli theorem](../../../../../../tonelli-theorem.md) and the planar [Brownian transition density](../../../../../../brownian-transition-density.md),

$$
\mathbb E[A_t]
=\int_0^t\mathbb E[f(X_s)]\,ds.
$$

For $s\geq1$,

$$
\mathbb E[f(X_s)]
=\int_{\mathbb R^2}f(y)\frac1{2\pi s}
e^{-|y-X_0|^2/(2s)}\,dy
\leq\frac1{2\pi s},
$$

while for $0\leq s\leq1$ it is at most $\|f\|_\infty$. Hence

$$
\mathbb E[A_t]\leq\|f\|_\infty+\frac{\log t}{2\pi}
$$

for $t\geq1$, and consequently

$$
\boxed{\mathbb E[A_t/t]\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
