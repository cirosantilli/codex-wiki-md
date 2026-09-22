<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed $t$, put $g_t(u)=(u-t)_+^{k-1}$, a [truncated power function](../../../../../../truncated-power-function.md). Begin with distinct increasing knots. The two [interpolation polynomials](../../../../../../interpolation-polynomial.md) $\ell_i(\cdot,t)$ and $\ell_{i+1}(\cdot,t)$ agree at their $k-1$ shared knots. Their difference has degree at most $k-1$, so

$$
\ell_{i+1}(x,t)-\ell_i(x,t)=c_i(t)\prod_{j=1}^{k-1}(x-t_{i+j})
=c_i(t)\omega_i(x).
$$

For $k=1$ the empty product is one and the same assertion holds for constant interpolants. The [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md) of a degree-at-most-$k-1$ interpolant on $k$ nodes is its order-$k-1$ [divided difference](../../../../../../divided-difference.md), by the [Newton interpolation polynomial](../../../../../../newton-polynomial.md). Therefore

$$
c_i(t)=[t_{i+1},\ldots,t_{i+k}]g_t-[t_i,\ldots,t_{i+k-1}]g_t
=(t_{i+k}-t_i)[t_i,\ldots,t_{i+k}]g_t=N_i(t).
$$

This proves the [Lee interpolation identity](../../../../../../lee-interpolation-identity.md)

$$
\boxed{\omega_i(x)N_i(t)=\ell_{i+1}(x,t)-\ell_i(x,t).}
$$

The identity holds for every real $x,t$, with the usual convention for the order-zero truncated power. Admissible repeated knots are handled by the corresponding confluent [divided differences](../../../../../../divided-difference.md) and consistent one-sided limits at breakpoints; taking these limits preserves the [Lee interpolation identity](../../../../../../lee-interpolation-identity.md).

Sum over $i$ to telescope:

$$
\sum_{i=1}^n\omega_i(x)N_i(t)=\ell_{n+1}(x,t)-\ell_1(x,t).
$$

If $t_k<t<t_{n+1}$, the first $k$ knot values of $g_t$ are zero, so $\ell_1=0$. At the last $k$ knots $t_{n+1},\ldots,t_{n+k}$, the function $g_t$ agrees with the [polynomial](../../../../../../polynomial-split.md) $(u-t)^{k-1}$, so uniqueness of [polynomial interpolation](../../../../../../polynomial-interpolation.md) gives $\ell_{n+1}(x,t)=(x-t)^{k-1}$. Thus the [Marsden identity](../../../../../../marsden-identity.md) is

$$
\boxed{(x-t)^{k-1}=\sum_{i=1}^n\omega_i(x)N_i(t),
\qquad t_k<t<t_{n+1},\quad x\in\mathbb R.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
