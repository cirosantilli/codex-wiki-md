<h1 id="18d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For node $x_i$, let $\ell_i$ be the [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) with $\ell_i(x_j)=\delta_{ij}$. It has degree $n$, so $\ell_i^2$ has degree $2n$. The [Gaussian quadrature](../../../../../../gaussian-quadrature.md) with $n+1$ nodes is exact through degree $2n+1$, hence

$$
a_i=\sum_{j=0}^na_j\ell_i(x_j)^2=\int_{-1}^1\ell_i(x)^2w(x)dx.
$$

The integrand is nonnegative. Since $\ell_i$ is a nonzero [polynomial](../../../../../../polynomial-split.md), it is nonzero on some open subinterval; the positive weight has positive [integral](../../../../../../integral.md) there. Consequently $\boxed{a_i>0}$ for every node. This proves the [positive weights of Gaussian quadrature](../../../../../../positive-weights-of-gaussian-quadrature.md) property without assuming any coefficient sign beforehand.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18D](../../18d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
