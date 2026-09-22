<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $E=f_H(\psi)$. For any admissible variation $\eta$, differentiation with respect to a real parameter gives

$$
\left.\frac d{dt}f_H(\psi+t\eta)\right|_{t=0}
=\frac{2\operatorname{Re}\langle\eta|(H-E)\psi\rangle}{\|\psi\|^2}.
$$

Stationarity for all variations, including their imaginary multiples, forces $(H-E)\psi=0$; conversely this [eigenvector](../../../eigenvector.md) equation makes the [derivative](../../../derivative.md) vanish. Thus **stationary [Rayleigh quotients](../../../rayleigh-quotient.md) are exactly [eigenvectors](../../../eigenvector.md), with their [eigenvalues](../../../eigenvalue.md) as the quotient values**.

Put $\kappa=e^2/(4\pi\epsilon_0)$ and assume $\alpha>0$. The squared [norm](../../../norm.md) of the radial trial function is $4\pi\int_0^\infty r^2e^{-2\alpha r}\,dr=\pi/\alpha^3$. Its kinetic expectation, computed through $\int|\nabla\psi|^2$, is $\hbar^2\alpha^2/(2m)=\kappa a\alpha^2/2$. Splitting the potential [integral](../../../integral-split.md) at $R$ gives

$$
\langle V\rangle=-4\kappa\alpha^3
\left(\frac1R\int_0^Rr^2e^{-2\alpha r}\,dr
+\int_R^\infty re^{-2\alpha r}\,dr\right)
=-\frac\kappa R\left[1-(1+\alpha R)e^{-2\alpha R}\right].
$$

For example, the first [integral](../../../integral-split.md) is $[1-e^{-2s}(1+2s+2s^2)]/(4\alpha^3)$ and the second is $e^{-2s}(R/(2\alpha)+1/(4\alpha^2))$, where $s=\alpha R$. Therefore

$$
\boxed{f_H(\psi_\alpha)=\kappa\left[\frac{a\alpha^2}{2}
-\frac{1-(1+\alpha R)e^{-2\alpha R}}R\right].}
$$

Its [derivative](../../../derivative.md) is $\kappa[a\alpha-(1+2\alpha R)e^{-2\alpha R}]$. The actual stationary condition is consequently

$$
\boxed{a\alpha=(1+2\alpha R)e^{-2\alpha R}.}
$$

The extra Coulomb factor in the printed stationary equation is an error: the common prefactor cancels on differentiation. The corrected equation is dimensionless on both sides. Its left side increases from zero, while its right side decreases from one, so it has one positive solution and gives the minimum in this trial family.

Let $\varepsilon=R/a$ and $y=a\alpha$. Expansion of $(1+2s)e^{-2s}$ gives $1-2s^2+O(s^3)$. Thus

$$
\boxed{a\alpha=1-2\varepsilon^2+O(\varepsilon^3),\qquad
\alpha=\frac1a\left[1-2(R/a)^2+O((R/a)^3)\right].}
$$

There is no linear correction in $R/a$. By the [quantum variational principle](../../../quantum-variational-principle.md), any normalized trial state gives an upper bound on the true ground energy. Choosing $\alpha=1/a$ already gives the exact bound

$$
\boxed{E_0(R)\leq\frac\kappa a\left[\frac12-
\frac{1-(1+\varepsilon)e^{-2\varepsilon}}{\varepsilon}\right].}
$$

Its small-radius expansion is

$$
E_0(R)\leq\frac\kappa a
\left[-\frac12+\frac23\varepsilon^2+O(\varepsilon^3)\right].
$$

Using the optimized $\alpha$ improves this bound starting at order $\varepsilon^4$, and hence gives the same leading finite-size correction. The true energy is also at least the point-nucleus value $-\kappa/(2a)$, since the finite-radius potential is nowhere more attractive.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2010](../../2010-split.md)
3. [Past exam of the quantum theory and quantum computers course of the University of Oxford](../../split.md)
4. [Quantum theory and quantum computers course of the University of Oxford](../../../quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
5. [Year 4 of the mathematics course of the University of Oxford](../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
