<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each $k\geq0$, monotonicity gives the dyadic-block bounds

$$
2^k x_{2^{k+1}}
\leq\sum_{n=2^k}^{2^{k+1}-1}x_n
\leq2^k x_{2^k}.
$$

Summing the upper bounds proves convergence of $\sum x_n$ whenever $\sum2^kx_{2^k}$ converges. Summing the lower bounds gives, up to the first term,

$$
\sum_{k\geq0}2^kx_{2^{k+1}}
=\frac12\sum_{j\geq1}2^jx_{2^j},
$$

so convergence of $\sum x_n$ forces convergence of the condensed series. This is the [Cauchy condensation test](../../../../../../cauchy-condensation-test.md):

$$
\boxed{\sum_{n\geq1}x_n\text{ converges}
\iff\sum_{k\geq0}2^kx_{2^k}\text{ converges}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
