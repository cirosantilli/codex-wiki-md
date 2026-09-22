<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $H_k=\sum_{j=1}^k1/j$, with $H_0=0$. The truncated uniform [prior](../../../../../../prior-probability.md) gives the [posterior distribution](../../../../../../bayesian-posterior.md)

$$
p(N\mid y,M)=\frac{N^{-1}}{H_M-H_{y-1}},\qquad y\leq N\leq M.
$$

Its [posterior mean](../../../../../../posterior-mean.md) is

$$
\boxed{\mathbb E[N\mid y,M]=\frac{M-y+1}{H_M-H_{y-1}}.}
$$

Each term in the numerator of the expectation is $N/N=1$, which explains the exact count $M-y+1$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
