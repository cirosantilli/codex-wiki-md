<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Seek a nonzero separated solution $\psi=T(t)R(r)\Theta(\theta)$. Substitution into the [heat equation](../../../../../heat-equation.md) and division by the product gives

$$
\frac{T'}{\kappa T}=\frac{(r^2R')'}{r^2R}+\frac{1}{r^2\Theta\sin\theta}(\sin\theta\,\Theta')'.
$$

The left side depends only on time, so set it to $-k^2$. Multiplication by $r^2$ then separates the angular dependence, with separation constant $\ell(\ell+1)$. The three [ordinary differential equations](../../../../../ordinary-differential-equation.md) are

$$
\boxed{T'+\kappa k^2T=0,}
$$



$$
\boxed{\frac1{\sin\theta}(\sin\theta\,\Theta')'+\ell(\ell+1)\Theta=0,}
$$



$$
\boxed{(r^2R')'+[k^2r^2-\ell(\ell+1)]R=0.}
$$

The temporal solution is $T=T_0e^{-\kappa k^2t}$. With $q=\cos\theta$, the angular equation is the [Legendre differential equation](../../../../../legendre-differential-equation.md); regularity at both angular endpoints selects $\ell=0,1,2,\ldots$ and $\Theta\propto P_\ell(q)$, the [Legendre polynomial](../../../../../legendre-polynomial.md). The radial equation has the [Spherical Bessel functions](../../../../../spherical-bessel-function.md) $j_\ell(kr)$ and $y_\ell(kr)$ for $k>0$. Regularity at $r=0$, if imposed, excludes the singular second solution. For $k=0$ the radial powers are $r^\ell$ and $r^{-\ell-1}$. Without specified radial [boundary conditions](../../../../../boundary-condition.md), no discrete set of $k$ is selected; $-k^2$ is a convention for the temporal separation constant.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
