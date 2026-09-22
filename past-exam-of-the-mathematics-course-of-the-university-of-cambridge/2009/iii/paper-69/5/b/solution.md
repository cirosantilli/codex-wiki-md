<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $d=k-1$ and let $e_m$ be the [elementary symmetric polynomial](../../../../../../elementary-symmetric-polynomial.md) of degree $m$ in the $d$ interior [spline knots](../../../../../../spline-knot.md) $t_{i+1},\ldots,t_{i+d}$, with $e_0=1$. Expanding the knot polynomial gives

$$
\omega_i(x)=\prod_{r=1}^d(x-t_{i+r})
=\sum_{m=0}^d(-1)^m e_m(t_{i+1},\ldots,t_{i+d})x^{d-m}.
$$

Compare the coefficient of $x^{d-m}$ in the [Marsden identity](../../../../../../marsden-identity.md). The left coefficient is $(-1)^m\binom dm t^m$; the right coefficient is $(-1)^m\sum_i e_m(t_{i+1},\ldots,t_{i+d})N_i(t)$. Cancelling the common sign therefore gives the [monomial B-spline coefficients](../../../../../../monomial-b-spline-coefficients.md):

$$
\boxed{a_i^{(m)}=\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}},\qquad 0\le m\le k-1.}
$$

Equivalently, for $m\ge1$ the numerator is $\sum_{1\le r_1<\cdots<r_m\le k-1}t_{i+r_1}\cdots t_{i+r_m}$. In particular $a_i^{(0)}=1$, so the order-zero case reproduces constants, and for $k\ge2$ the linear coefficients are $a_i^{(1)}=(t_{i+1}+\cdots+t_{i+k-1})/(k-1)$, the [Greville abscissae](../../../../../../greville-abscissa.md). At $m=k-1$, the coefficient is the product of all interior knots. Each formula holds on the basic knot interval used in the [Marsden identity](../../../../../../marsden-identity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
