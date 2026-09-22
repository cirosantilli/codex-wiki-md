<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The appropriate [weighted inner product](../../../../../weighted-inner-product.md) and [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) are

$$
\boxed{\langle u,v\rangle_w=\int_1^R x^2\overline{u(x)}v(x)\,dx,\qquad
Lv=\frac1{x^2}\left[-(x(x-1)v')'+l(l+1)v\right].}
$$

For two functions obeying the endpoint conditions, [integration by parts](../../../../../integration-by-parts.md) gives the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md)

$$
\langle u,Lv\rangle_w-\langle Lu,v\rangle_w
=\left[x(x-1)(\overline{u'}v-\overline u v')\right]_1^R=0.
$$

At $R$, both $u$ and $v$ vanish. At $1$, the factor $x(x-1)$ tends to zero while the functions and their first [derivatives](../../../../../derivative.md) remain bounded. Thus the boundary form vanishes at both ends.

This gives the regular [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md) realization: its singular-end condition is $\lim_{x\downarrow1}x(x-1)v'=0$, together with $v(R)=0$. The bounded classical [eigenfunctions](../../../../../eigenfunction.md) satisfy exactly this no-log choice. More precisely the operator domain is the maximal differential-operator domain in the weighted space with these separated endpoint conditions; the preceding calculation verifies its self-adjoint boundary form, rather than merely the differential expression's formal symmetry.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
