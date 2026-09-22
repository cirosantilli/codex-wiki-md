<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A $C^2$ piecewise cubic supported on $[0,ph]$ has the truncated-power representation with indices $0,\ldots,p$. Vanishing for $x\geq ph$ imposes

$$
\sum_{j=0}^pa_jj^m=0,\qquad m=0,1,2,3,
$$

after expanding its cubic exterior [polynomial](../../../../../polynomial-split.md); powers of $h$ cancel. For $p\leq3$, the [Vandermonde matrix](../../../../../vandermonde-matrix.md) columns are independent, forcing every coefficient to be zero. For $p=4$, coefficients proportional to $(1,-4,6,-4,1)$ satisfy these conditions because a fourth finite difference annihilates cubics.

Normalize to get the [Cardinal cubic B-spline](../../../../../cardinal-cubic-b-spline.md)

$$
\boxed{N_0^3(x)=\frac1{6h^3}\sum_{j=0}^4(-1)^j\binom4j(x-jh)_+^3.}
$$

At its five support knots its values are $0,1/6,2/3,1/6,0$, so their sum is one. Thus **four intervals are necessary and sufficient**.

For $h=1/2$, the five translates active in the interior of $[0,1]=[0,2h]$ are indexed $-3,-2,-1,0,1$. Write $s(x)=\sum_{j=-3}^1c_jN_j^3(x)$. Nodal [interpolation](../../../../../interpolation-split.md) gives

$$
\begin{aligned}
c_{-3}+4c_{-2}+c_{-1}&=6u(0),\\
c_{-2}+4c_{-1}+c_0&=6u(h),\\
c_{-1}+4c_0+c_1&=6u(2h).
\end{aligned}
$$

At the left endpoint the first [derivatives](../../../../../derivative.md) of the three active [functions](../../../../../function-split.md) are $-1/(2h),0,1/(2h)$, and their second [derivatives](../../../../../derivative.md) are $1/h^2,-2/h^2,1/h^2$. The two remaining equations are

$$
\boxed{c_{-1}-c_{-3}=2h\,u'(0),\qquad
c_{-3}-2c_{-2}+c_{-1}=h^2u''(0).}
$$

Together these five equations form the requested system; insert $h=1/2$ if numerical coefficients are desired. The first, fourth and fifth determine the first three coefficients, and the other two then determine $c_0,c_1$, so the system is nonsingular.

The source only assumes $u\in C[0,1]$, which need not have either endpoint [derivative](../../../../../derivative.md). The Hermite conditions require those [derivatives](../../../../../derivative.md) to exist, or to be supplied as separate [interpolation](../../../../../interpolation-split.md) data. The nodal conditions alone remain meaningful for every continuous $u$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
