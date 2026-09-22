<h1 id="c/c2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $\gcd(b,c)>1$, both [Jacobi symbols](../../../../../../jacobi-symbol.md) vanish, so the formula holds. Otherwise write $b=\prod_i p_i$ and $c=\prod_j q_j$, retaining repeated factors. [Multiplicativity of the Jacobi symbol](../../../../../../multiplicativity-of-the-jacobi-symbol.md) and [quadratic reciprocity](../../../../../../quadratic-reciprocity.md) give

$$
\left(\frac bc\right)
=\prod_{i,j}\left(\frac{p_i}{q_j}\right)
=\prod_{i,j}\left(\frac{q_j}{p_i}\right)
(-1)^{\sum_{i,j}(p_i-1)(q_j-1)/4}.
$$

The exponent is

$$
\left(\sum_i\frac{p_i-1}2\right)
\left(\sum_j\frac{q_j-1}2\right)
\equiv\frac{b-1}2\frac{c-1}2\pmod2
$$

by the parity identity from part (i). The product of the reversed [Legendre symbols](../../../../../../legendre-symbol.md) is $(c/b)$. Thus the [Jacobi reciprocity law](../../../../../../jacobi-reciprocity-law.md) is

$$
\boxed{\left(\frac bc\right)=\left(\frac cb\right)(-1)^{(b-1)(c-1)/4}.}
$$

This also covers $b=1$ or $c=1$ by empty products.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [C2](../../../c2.md)
4. [C](../../../../c.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
