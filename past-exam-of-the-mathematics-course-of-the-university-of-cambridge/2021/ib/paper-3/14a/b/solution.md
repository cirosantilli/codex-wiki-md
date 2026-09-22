<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplication by $(1-x^2)^k$ puts the equation in [self-adjoint form](../../../../../../self-adjoint-differential-equation.md):

$$
\boxed{
\frac d{dx}\left[(1-x^2)^{k+1}Q_k'\right]
+\lambda_k(1-x^2)^kQ_k=0
}.
$$

Multiply by $Q_k$ and integrate over $[-1,1]$. Regularity and the vanishing factor at both endpoints remove the boundary term in [integration by parts](../../../../../../integration-by-parts.md), leaving

$$
\int_{-1}^1(1-x^2)^{k+1}(Q_k')^2\,dx
=\lambda_k\int_{-1}^1(1-x^2)^kQ_k^2\,dx.
$$

If $Q_k$ is not identically zero, the integral on the right without $\lambda_k$ is positive, whereas the left side is nonnegative. Therefore

$$
\boxed{\lambda_k\geq0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
