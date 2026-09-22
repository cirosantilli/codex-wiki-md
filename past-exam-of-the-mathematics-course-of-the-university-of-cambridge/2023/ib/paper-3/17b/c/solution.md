<h1 id="17b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each node $x_i^{(n)}$, let

$$
\ell_i(x)=\prod_{j\ne i}
\frac{x-x_j^{(n)}}{x_i^{(n)}-x_j^{(n)}}
$$

be its [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md). It has degree $n$ and satisfies $\ell_i(x_j^{(n)})=\delta_{ij}$. Since $\ell_i^2\in\mathcal P_{2n}$, exactness gives

$$
a_i^{(n)}=I_n(\ell_i^2)=I(\ell_i^2)
=\int_a^b\ell_i(x)^2w(x)\,dx.
$$

The integrand is nonnegative and is positive except at finitely many points, so

$$
\boxed{a_i^{(n)}>0}.
$$

This proves the [positivity of quadrature weights from degree 2n exactness](../../../../../../positivity-of-quadrature-weights-from-degree-2n-exactness.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
