<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [separation of variables](../../../../../separation-of-variables.md), writing $\Psi=F(r)\Theta(\theta)$. After multiplication by $r^2/(F\Theta)$, the radial and angular terms are functions of independent variables, so set

$$
\frac{(r^2F')'}F=-\frac{(\sin\theta\,\Theta')'}{\sin\theta\,\Theta}=\lambda.
$$

With $x=\cos\theta$, the angular equation is

$$
\frac d{dx}\left[(1-x^2)\frac{d\Theta}{dx}\right]+\lambda\Theta=0.
$$

Regularity at both poles selects $\lambda=\ell(\ell+1)$, $\ell=0,1,\ldots$, and the [Legendre polynomials](../../../../../legendre-polynomial.md) $P_\ell(x)$; the other angular branch is singular at a pole. The radial [Euler-Cauchy equation](../../../../../euler-cauchy-equation.md) is $r^2F''+2rF'-\ell(\ell+1)F=0$. A power $r^s$ gives $(s-\ell)(s+\ell+1)=0$, hence $F=a_\ell r^\ell+b_\ell r^{-\ell-1}$.

Superposing these axisymmetric [spherical harmonics](../../../../../spherical-harmonic.md) gives

$$
\boxed{\Psi(r,\theta)=\sum_{\ell=0}^\infty\left(a_\ell r^\ell+\frac{b_\ell}{r^{\ell+1}}\right)P_\ell(\cos\theta).}
$$

The coefficients must give convergence appropriate to the domain. In a region containing the origin, regularity removes the negative powers; in an exterior region with zero potential at infinity, it removes the growing powers and the constant. No such radial restriction is needed for a general annular region.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
