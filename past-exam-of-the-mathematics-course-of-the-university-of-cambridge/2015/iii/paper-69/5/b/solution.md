<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $d=k-1$ and let $e_m(t_{i+1},\ldots,t_{i+d})$ be the [elementary symmetric polynomial](../../../../../../elementary-symmetric-polynomial.md) of degree $m$ in the interior knots, with $e_0=1$. Expand the [Marsden identity](../../../../../../marsden-identity.md) in powers of $x$. The coefficient of $x^{d-m}$ on the left is $(-1)^m\binom dm t^m$; that coefficient in $\omega_i(x)$ is $(-1)^me_m(t_{i+1},\ldots,t_{i+d})$. Comparing and cancelling the sign proves **the [monomial B-spline coefficients](../../../../../../monomial-b-spline-coefficients.md)**:

$$
\boxed{a_i^{(m)}=\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}},\qquad0\leq m\leq k-1.}
$$

For $m=0$ this gives [partition of unity](../../../../../../partition-of-unity.md) on the basic interval. For $m=1$ it gives the [Greville abscissae](../../../../../../greville-abscissa.md), the arithmetic means of the $k-1$ interior knots. For the top degree it gives their product. When $k=1$, only $m=0$ occurs and the empty symmetric [polynomial](../../../../../../polynomial-split.md) is one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
