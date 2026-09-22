<h1 id="20/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply the two displayed equations by $e^{-x}$ and subtract the one with indices reversed. The product terms combine into the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md):

$$
\frac{d}{dx}\left[xe^{-x}(L_mL_n'-L_nL_m')\right]
+(n-m)e^{-x}L_mL_n=0.
$$

Integrating from zero to infinity gives

$$
\left[xe^{-x}(L_mL_n'-L_nL_m')\right]_0^\infty
+(n-m)\int_0^\infty e^{-x}L_mL_n\,dx=0.
$$

All factors $L_j,L_j'$ are [polynomials](../../../../../polynomial-split.md). The endpoint term at zero vanishes because of the factor $x$, and the one at infinity vanishes because the [exponential function](../../../../../exponential-function.md) dominates every [polynomial](../../../../../polynomial-split.md). Therefore, if $m\ne n$,

$$
\boxed{\int_0^\infty e^{-x}L_m(x)L_n(x)\,dx=0}.
$$

The [integral](../../../../../integral-split.md) is absolutely convergent. This is [orthogonality](../../../../../orthogonal-vectors.md) in the [weighted inner product](../../../../../weighted-inner-product.md) with weight $e^{-x}$; the [boundary](../../../../../boundary-of-a-set.md) cancellation is the self-adjoint mechanism behind the [Laguerre differential operator on polynomials](../../../../../laguerre-differential-operator-on-polynomials.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
