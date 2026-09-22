<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For two real [eigenfunctions](../../../../eigenfunction.md), multiply the equation for $y_n$ by $y_m$ and the equation for $y_m$ by $y_n$, then subtract. The $q$ terms cancel. The resulting [Lagrange identity for a Sturm-Liouville operator](../../../../lagrange-identity-for-a-sturm-liouville-operator.md) is

$$
\left[p(y_my_n'-y_ny_m')\right]'+(\lambda_n-\lambda_m)r y_my_n=0.
$$

Integrating first over $[\epsilon,R]$ and then taking the endpoint limits gives

$$
(\lambda_n-\lambda_m)\int_0^\infty r y_my_n\,dx=-\left[p(y_my_n'-y_ny_m')\right]_0^\infty.
$$

The needed assumptions are that the [improper integral](../../../../improper-integral.md) exists and that the displayed boundary expression tends to zero at both endpoints. Bounded $y_m,y_n$ and their first [derivatives](../../../../derivative.md) are sufficient because $p\to0$, but are stronger than necessary. Merely knowing that $p\to0$ does not control arbitrarily growing [eigenfunctions](../../../../eigenfunction.md). With the vanishing boundary form and distinct [eigenvalues](../../../../eigenvalue.md), division by $\lambda_n-\lambda_m$ proves [orthogonality of Sturm-Liouville eigenfunctions](../../../../orthogonality-of-sturm-liouville-eigenfunctions.md):

$$
\boxed{\int_0^\infty r(x)y_m(x)y_n(x)\,dx=0\quad(m\ne n).}
$$

For complex [eigenfunctions](../../../../eigenfunction.md) in a real [self-adjoint differential operator](../../../../self-adjoint-differential-operator.md) problem, use $\overline{y_m}$ instead, giving the corresponding [weighted inner product](../../../../weighted-inner-product.md).

Multiplying the particular equation by $e^{-x}$ puts it in [Sturm-Liouville form](../../../../sturm-liouville-form.md):

$$
(xe^{-x}y')'+\lambda e^{-x}y=0.
$$

Consequently

$$
\boxed{p(x)=xe^{-x},\qquad q(x)=0,\qquad r(x)=e^{-x}.}
$$

Its polynomial [eigenfunctions](../../../../eigenfunction.md) are the [Laguerre polynomials](../../../../laguerre-polynomial.md). Products of these [polynomials](../../../../polynomial-split.md), with or without one [derivative](../../../../derivative.md), grow only algebraically at infinity. The exponential in $p$ therefore makes the boundary form vanish there; its factor $x$ makes it vanish at zero. Their [orthogonality](../../../../orthogonal-vectors.md) is thus

$$
\int_0^\infty e^{-x}y_m(x)y_n(x)\,dx=0\quad(m\ne n).
$$

For $\lambda=1$, substitution of $Ax+B$ gives $A+B=0$. For $\lambda=2$, substitution of $Ax^2+Bx+C$ gives $4A+B=0$ and $B+2C=0$. Choosing $y_n(0)=1$, which fixes the otherwise arbitrary nonzero multiplicative constants, yields

$$
\boxed{y_1=1-x,\qquad y_2=1-2x+\frac{x^2}{2}.}
$$

Their product is $1-3x+\tfrac52x^2-\tfrac12x^3$. Using the [Gamma function](../../../../gamma-function.md) identity $\int_0^\infty x^ke^{-x}dx=k!$, also obtainable by repeated [integration by parts](../../../../integration-by-parts.md), verifies the required [orthogonality](../../../../orthogonal-vectors.md) directly:

$$
\int_0^\infty e^{-x}y_1y_2\,dx=1-3(1!)+\frac52(2!)-\frac12(3!)=0.
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
