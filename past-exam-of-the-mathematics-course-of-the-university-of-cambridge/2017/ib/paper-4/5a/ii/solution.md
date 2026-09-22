<h1 id="5a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This subpart is also present in the original PDF but missing from the local TeX. Put $p(x)=1-x^2$ and $\lambda_n=n(n+1)$. Multiply the [Legendre differential equation](../../../../../../legendre-differential-equation.md) for $P_n$ by $P_m$, multiply the equation for $P_m$ by $P_n$, and subtract. The [product rule](../../../../../../product-rule.md) gives

$$
\frac{d}{dx}\bigl[p(P_mP_n'-P_nP_m')\bigr]
+(\lambda_n-\lambda_m)P_nP_m=0.
$$

Integrating from $-1$ to $1$, the boundary term vanishes: $p(\pm1)=0$, and the [Legendre polynomials](../../../../../../legendre-polynomial.md) and their [derivatives](../../../../../../derivative.md) are finite there. For distinct nonnegative [integers](../../../../../../integer.md) $m,n$, $\lambda_m\ne\lambda_n$. Thus the [Orthogonality of Legendre polynomials](../../../../../../orthogonality-of-legendre-polynomials.md) is

$$
\boxed{\int_{-1}^1P_m(x)P_n(x)\,dx=0\quad(m\ne n)}.
$$

The vanishing coefficient at the endpoints causes no difficulty here because the solutions are [polynomials](../../../../../../polynomial-split.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5A](../../5a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
