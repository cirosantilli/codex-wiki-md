<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For this part relabel one consecutive block of $k+1$ distinct knots as $t_0,\ldots,t_k$. This is a local reindexing; no extra global knot is being introduced. Let $g_t(u)=(u-t)_+^{k-1}$. Its [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) through the knot values is

$$
\ell(u)=\sum_{i=0}^kg_t(t_i)\frac{\omega(u)}{(u-t_i)\omega'(t_i)},\qquad
\omega(u)=\prod_{j=0}^k(u-t_j).
$$

Each quotient $\omega(u)/(u-t_i)$ is monic of degree $k$. Comparing [leading coefficients](../../../../../../leading-coefficient-of-a-polynomial.md) gives

$$
[u^k]\ell(u)=\sum_{i=0}^k\frac{g_t(t_i)}{\omega'(t_i)}.
$$

The same [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md) is the order-$k$ [divided difference](../../../../../../divided-difference.md) $[t_0,\ldots,t_k]g_t$, by the [Newton interpolation polynomial](../../../../../../newton-polynomial.md) representation. Multiplying by $k$ therefore gives the explicit [B-spline](../../../../../../b-spline.md) formula

$$
\boxed{M_0(t)=k\sum_{i=0}^k\frac{(t_i-t)_+^{k-1}}{\omega'(t_i)}.}
$$

Distinct knots make every denominator nonzero. For $k=1$ the degree-zero truncated power is interpreted as an interval-indicator convention; values at individual endpoints do not affect its integral.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
