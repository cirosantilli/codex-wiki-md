<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A cubic [spline](../../../../../spline-mathematics.md) that vanishes for $x\leq0$ and is twice continuously differentiable can be written using [truncated power functions](../../../../../truncated-power-function.md) as $s(x)=\sum_{j=0}^k a_j(x-jh)_+^3$. Vanishing for $x\geq kh$ imposes the four moment equations $\sum_j a_jj^r=0$ for $r=0,1,2,3$. Their [Vandermonde matrix](../../../../../vandermonde-matrix.md) has rank $\min(4,k+1)$, so a nonzero coefficient vector first exists at $\boxed{k=4}$.

A normalized compact [cubic cardinal B-spline](../../../../../cubic-cardinal-b-spline.md) is

$$
\boxed{B_3(x/h)=\frac16\sum_{j=0}^4(-1)^j\binom4j(x/h-j)_+^3.}
$$

It has nodal values $0,1/6,2/3,1/6,0$ at $0,h,2h,3h,4h$, so their sum is one. The alternating [binomial coefficients](../../../../../binomial-coefficient-split.md) meet the four moment equations, and the factor $1/6$ fixes the requested normalization.

For interpolation on $[-1,1]$, centre the translates as $\beta_j(x)=B_3(x/h-j+2)$, with $j=-n-1,\ldots,n+1$. Their restrictions form a [basis](../../../../../basis.md) for the cubic $C^2$ [spline](../../../../../spline-mathematics.md) space on these knots. Write $S=\sum_jc_j\beta_j$. The $2n+1$ interpolation equations are

$$
\boxed{\frac{c_{r-1}+4c_r+c_{r+1}}6=u(rh),\qquad r=-n,\ldots,n.}
$$

The recurrence determines all remaining coefficients after choosing $c_{-n-1},c_{-n}$, giving exactly two free parameters. The two [natural cubic spline](../../../../../natural-cubic-spline.md) conditions become

$$
\boxed{c_{-n-1}-2c_{-n}+c_{-n+1}=0,\qquad c_{n-1}-2c_n+c_{n+1}=0,}
$$

because $S''(rh)=h^{-2}(c_{r-1}-2c_r+c_{r+1})$.

For uniqueness, take the difference $s$ of two candidates. It vanishes at every knot and has $s''(\pm1)=0$. Integrating by parts twice on each cubic piece gives $\int_{-1}^1(s'')^2=0$: terms involving $s$ vanish at the knots, and those involving $s''s'$ cancel at internal knots and vanish at the endpoints. Thus $s''=0$; the remaining affine [function](../../../../../function-split.md) vanishes at both endpoints and is zero. The square linear system for the coefficients is therefore nonsingular, giving existence as well as uniqueness of the [natural cubic spline interpolant](../../../../../natural-cubic-spline-interpolant.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
