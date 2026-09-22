<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The covariance is

$$
\mathbb E[\Gamma(x)\Gamma(y)]
=\frac12G_{\{a\}}(x,y).
$$

Indeed, the killed-walk Green function satisfies

$$
G_{\{a\}}(x,y)
=\mathbf1_{\{x=y\}}+\frac1{2d}\sum_{z\sim x}G_{\{a\}}(z,y),
\qquad G_{\{a\}}(a,y)=0.
$$

On the other hand, the conditional mean from part 2 makes the covariance harmonic in $x\ne y,a$. At $x=y$, the conditional variance $1/2$ gives the same equation with source $\frac12\mathbf1_{\{x=y\}}$. Uniqueness of the [Dirichlet problem](../../../../../../dirichlet-problem.md) therefore identifies the covariance with $G_{\{a\}}/2$. The factor $1/2$ comes from the coefficient $1/(2d)$ in this paper's energy density.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
