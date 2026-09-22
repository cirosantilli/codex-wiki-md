<h1 id="40a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $D=-10I/(3h^2)$ be the diagonal part of $A$. The [weighted Jacobi method](../../../../../../weighted-jacobi-method.md) is

$$
\boxed{u^{(r+1)}=(1-\omega)u^{(r)}+\omega D^{-1}[b-(A-D)u^{(r)}].}
$$

Equivalently it is $u^{(r+1)}=u^{(r)}+\omega D^{-1}(b-Au^{(r)})$. In grid form, all neighbours on the right are taken from the old iterate:

$$
\boxed{u_{ij}^{(r+1)}=(1-\omega)u_{ij}^{(r)}+\omega\left[\frac15\sum_{\rm axial}u^{(r)}+\frac1{20}\sum_{\rm diagonal}u^{(r)}-\frac{3h^2}{10}f_{ij}\right].}
$$

The boundary values stay zero at every step. The iteration matrix is $T_\omega=I-\omega D^{-1}A$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [40A](../../40a.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
