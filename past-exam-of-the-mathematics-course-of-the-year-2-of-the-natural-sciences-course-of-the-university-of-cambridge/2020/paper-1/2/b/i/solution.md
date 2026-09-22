<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Substitute $U=R(r)F(\theta)$ into the axisymmetric [Laplace equation](../../../../../../laplace-equation.md) and multiply by $r^2/(RF)$. The radial and angular terms must be separate constants:

$$
\frac1R\frac d{dr}(r^2R')=-\frac1{F\sin\theta}\frac d{d\theta}(\sin\theta F')=\lambda.
$$

Thus

$$
r^2R''+2rR'-\lambda R=0,\qquad
\frac1{\sin\theta}(\sin\theta F')'+\lambda F=0.
$$

With $x=\cos\theta$, the angular equation becomes

$$
(1-x^2)F_{xx}-2xF_x+\lambda F=0.
$$

Requiring boundedness on the entire polar interval, and using the supplied characterization of bounded [Legendre polynomial](../../../../../../legendre-polynomial.md) solutions, gives $\lambda=n(n+1)$ and $F\propto P_n(\cos\theta)$ for $n=0,1,2,\ldots$. Trying $R=r^s$ gives $s(s+1)=n(n+1)$, hence $s=n$ or $s=-n-1$.

The globally angular-regular separated modes and their superposition are therefore

$$
\boxed{U_n=(A_nr^n+B_nr^{-n-1})P_n(\cos\theta),}
$$



$$
\boxed{U(r,\theta)=\sum_{n=0}^\infty(A_nr^n+B_nr^{-n-1})P_n(\cos\theta).}
$$

Coefficients and convergence are determined by the radial domain and boundary data. A domain containing the origin excludes negative radial powers for a regular solution. If the angular domain excludes a polar axis of the [spherical coordinate system](../../../../../../spherical-coordinate-system.md) and singular angular behavior is allowed, additional Legendre-function branches are possible; the displayed family is the one regular over the complete sphere, as intended by the hint.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
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
