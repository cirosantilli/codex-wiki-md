<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First move the order parameter term to the right-hand side:

$$
x^2y''+xy'+\beta^2x^2y=n^2y.
$$

Here $p=x^2$, $r=x$, so the [integrating factor](../../../../../../integrating-factor.md) obeys

$$
\frac{w'}w=\frac{r-p'}p=-\frac1x,
\qquad w(x)=\frac{C}{x}.
$$

Choose the irrelevant positive constant $C=1$. Multiplying the equation by $1/x$ gives

$$
(xy')'+\beta^2xy=\frac{n^2}{x}y.
$$

Thus a [Sturm-Liouville theory](../../../../../../sturm-liouville-theory-split.md) [eigenvalue](../../../../../../eigenvalue.md) formulation with the requested [eigenvalue](../../../../../../eigenvalue.md) is

$$
\boxed{Ly=\lambda wy,\qquad
L=\frac d{dx}\left(x\frac d{dx}\right)+\beta^2x,\quad
w=\frac1x,\quad\lambda=n^2.}
$$

This is the [Sturm-Liouville formulation with Bessel order as eigenvalue](../../../../../../sturm-liouville-formulation-with-bessel-order-as-eigenvalue.md). The spectral parameter is the squared order of the [Bessel function](../../../../../../bessel-function-split.md), with $\beta$ treated as fixed. This differs from the also familiar formulation in which $\beta^2$ is the [eigenvalue](../../../../../../eigenvalue.md).

The factor $1/x$ is singular at the origin. Consequently the [integral](../../../../../../integral-split.md) defining $w$ cannot literally use lower limit zero; take a positive reference point $x_*>0$, obtain $w=x_*/x$, and absorb $x_*$ into the normalization. The differential identity holds for $x>0$. [Boundary conditions](../../../../../../boundary-condition.md) and admissibility at zero and at the outer endpoint are additional ingredients needed to make a particular self-adjoint spectral problem.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
