<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a vacuum [electric potential](../../../../electric-potential.md), put $\Phi=R(r)Y(\theta)$ in [Laplace's equation](../../../../laplace-equation.md) in [spherical coordinates](../../../../spherical-coordinate-system.md). Multiplication by $r^2/(RY)$ separates the radial and angular terms. With separation constant $\ell(\ell+1)$ and $x=\cos\theta$, the angular [Legendre differential equation](../../../../legendre-differential-equation.md) is

$$
\boxed{\frac d{dx}\left[(1-x^2)\frac{dP_\ell}{dx}\right]+\ell(\ell+1)P_\ell=0.}
$$

Regularity at both polar axes selects nonnegative [integers](../../../../integer-split.md) $\ell$ and the [Legendre polynomials](../../../../legendre-polynomial.md). The radial equation is $(r^2R')'-\ell(\ell+1)R=0$, whose independent solutions are $r^\ell$ and $r^{-\ell-1}$. Hence the angularly regular axisymmetric vacuum solution is

$$
\boxed{\Phi(r,\theta)=\sum_{\ell=0}^\infty(A_\ell r^\ell+B_\ell r^{-\ell-1})P_\ell(\cos\theta).}
$$

The radial [domain](../../../../domain-mathematical-analysis.md) and its [boundary conditions](../../../../boundary-condition.md) determine which terms are admissible.

For the given [charge density](../../../../charge-density.md), only $P_1(\cos\theta)=\cos\theta$ is forced. Write $\Phi=f(r)\cos\theta$. The interior radial [Poisson equation](../../../../poisson-s-equation.md) is $f''+2f'/r-2f/r^2=-4$. The identity for the [Poisson equation with a spherical harmonic source](../../../../poisson-equation-with-a-spherical-harmonic-source.md) gives the particular solution $f_p=-r^2$, since the radial operator takes $r^2$ to four. Finiteness at zero and decay at infinity therefore give

$$
\Phi_{\rm in}=(Ar-r^2)\cos\theta,\qquad\Phi_{\rm out}=Br^{-2}\cos\theta.
$$

Continuity of the [electric potential](../../../../electric-potential.md) and its radial [derivative](../../../../derivative.md) at $a$ requires $Aa-a^2=B/a^2$ and $A-2a=-2B/a^3$. Solving gives $A=4a/3$, $B=a^4/3$, so

$$
\boxed{\Phi(r,\theta)=\begin{cases}(\tfrac43ar-r^2)\cos\theta,&0\leq r\leq a,\\\dfrac{a^4}{3r^2}\cos\theta,&r\geq a.\end{cases}}
$$

All other angular modes have zero coefficients after imposing regularity, matching and decay. At the origin the interior expression is $(4a/3)z-rz$, which extends with a continuous [gradient](../../../../gradient.md) and value zero. The angular [charge density](../../../../charge-density.md) has no unique value exactly at that point; [Poisson's equation](../../../../poisson-s-equation.md) holds classically for $r>0$ and as a [weak solution](../../../../weak-solution.md) through the origin. There is no additional point charge.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
