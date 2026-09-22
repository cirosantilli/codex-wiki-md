<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By spherical symmetry, choose the orbital plane to be $\theta=\pi/2$. The [geodesic Lagrangian](../../../../geodesic-lagrangian.md) of the [Schwarzschild metric](../../../../schwarzschild-spacetime-split.md) is

$$
\mathcal L=\frac12\left(-Bc^2\dot t^2+B^{-1}\dot r^2+r^2\dot\phi^2\right),
\qquad B=1-\frac{2GM}{rc^2}.
$$

For a massive [test particle](../../../../test-particle.md), dots denote [proper time](../../../../proper-time.md) derivatives and $2\mathcal L=-c^2$. The [cyclic coordinates](../../../../cyclic-coordinate.md) $t$ and $\phi$ give, through the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md), two constants:

$$
B\dot t=\mathcal E,\qquad r^2\dot\phi=\ell.
$$

At infinity, $\mathcal E=\gamma_\infty=1/\sqrt{1-v_\infty^2/c^2}$ is the [Lorentz factor](../../../../lorentz-factor.md). The constant $\ell$ is the [specific angular momentum](../../../../specific-angular-momentum.md), and the energy per unit [rest mass](../../../../invariant-mass.md) is $E_\infty/m=c^2\gamma_\infty$. The normalization of the [four-velocity](../../../../four-velocity.md) gives

$$
-c^2=-\frac{c^2\gamma_\infty^2}{B}
+\frac{\dot r^2}{B}+\frac{\ell^2}{r^2},
\qquad
\dot r^2=c^2\gamma_\infty^2-B\left(c^2+\frac{\ell^2}{r^2}\right).
$$

Use $dr/d\phi=\dot r\,r^2/\ell$ and define the [energy-normalized angular momentum for a Schwarzschild geodesic](../../../../energy-normalized-angular-momentum-for-a-schwarzschild-geodesic.md)

$$
J=\frac{\ell}{\gamma_\infty}=\frac{c^2L_\infty}{E_\infty}.
$$

Then

$$
\boxed{\left(\frac{dr}{d\phi}\right)^2
+r^2B\left(1+\frac{c^2r^2}{\gamma_\infty^2J^2}\right)
=\frac{c^2r^4}{J^2}.}
$$

For an incoming massive [test particle](../../../../test-particle.md) with [impact parameter](../../../../impact-parameter.md) $b$, $L_\infty=m\gamma_\infty v_\infty b$, so $J=bv_\infty$. In particular, $J$ is not the same as the [specific angular momentum](../../../../specific-angular-momentum.md) $\ell$ unless $\gamma_\infty=1$.

A [photon](../../../../photon.md) has no [proper time](../../../../proper-time.md) parametrization and no finite [Lorentz factor](../../../../lorentz-factor.md). For it, use an [affine parameter](../../../../affine-parameter.md) in the same [geodesic Lagrangian](../../../../geodesic-lagrangian.md) and impose $2\mathcal L=0$. The ratio $J=c^2L_\infty/E_\infty=bc$ remains well defined, and the null result is

$$
\boxed{\left(\frac{dr}{d\phi}\right)^2+r^2B=\frac{r^4}{b^2}.}
$$

Equivalently this is the ultrarelativistic limit of the massive formula at fixed $J$, with $1/\gamma_\infty^2\to0$. The printed massive formula needs this interpretation before it is applied to a [photon](../../../../photon.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
