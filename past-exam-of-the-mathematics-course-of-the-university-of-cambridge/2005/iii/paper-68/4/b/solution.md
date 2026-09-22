<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d=k-1$ and let $e_m$ denote the [elementary symmetric polynomial](../../../../../../elementary-symmetric-polynomial.md) of degree $m$ in the $d$ interior knots $t_{i+1},\ldots,t_{i+d}$, with $e_0=1$. Expand the two sides of the [Marsden identity](../../../../../../marsden-identity.md) as [polynomials](../../../../../../polynomial-split.md) in $x$:

$$
(x-t)^d=\sum_{m=0}^d(-1)^m\binom dm t^m x^{d-m},
$$

and

$$
\omega_i(x)=\prod_{j=1}^d(x-t_{i+j})
=\sum_{m=0}^d(-1)^m e_m(t_{i+1},\ldots,t_{i+d})x^{d-m}.
$$

Comparing the coefficient of $x^{d-m}$ and cancelling the common sign gives the [monomial B-spline coefficients](../../../../../../monomial-b-spline-coefficients.md)

$$
\boxed{a_i^{(m)}=
\frac{e_m(t_{i+1},\ldots,t_{i+k-1})}{\binom{k-1}{m}},
\qquad 0\leq m\leq k-1.}
$$

Equivalently,

$$
a_i^{(m)}=\binom{k-1}{m}^{-1}
\sum_{1\leq j_1<\cdots<j_m\leq k-1}
t_{i+j_1}\cdots t_{i+j_m}.
$$

In particular $a_i^{(0)}=1$, giving [partition of unity](../../../../../../partition-of-unity.md) on the interior interval. For $k\geq2$, $a_i^{(1)}=(t_{i+1}+\cdots+t_{i+k-1})/(k-1)$, and the highest-degree coefficient is the product of those interior knots. The formulas also cover $k=1,m=0$ through empty products.

## ↑ Ancestors (11)

1. [B](../b.md)
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
