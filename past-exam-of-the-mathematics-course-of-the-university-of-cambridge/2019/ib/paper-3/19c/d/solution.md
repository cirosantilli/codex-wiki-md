<h1 id="19c/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $x_1,\ldots,x_N$ be the distinct real roots of $\mathrm{He}_N$. The [Gauss-Hermite quadrature](../../../../../../gauss-hermite-quadrature.md) rule is

$$
\int_{-\infty}^{\infty}f(x)e^{-x^2/2}\,dx
\approx\sum_{j=1}^Nw_jf(x_j),
$$

where $w_j$ is the weighted integral of the $j$th [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md). Equivalently,

$$
w_j=\frac{N!\sqrt{2\pi}}{N^2\mathrm{He}_{N-1}(x_j)^2}>0.
$$

The orthogonality of $\mathrm{He}_N$ makes the rule exact for every polynomial of degree at most

$$
\boxed{2N-1}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [19C](../../19c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
