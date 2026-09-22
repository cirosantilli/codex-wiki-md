<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First check the printed equations literally. Set $v=0$ and use $\rho_0'/\rho_0=-1/H$. Differentiating continuity in time and using horizontal momentum gives

$$
p_{xx}=\rho_0(w_{zt}-w_t/H).
$$

Vertical momentum and [buoyancy](../../../../buoyancy.md) give $w_{tt}+N^2w=-p_{zt}/\rho_0$. Combining them therefore yields

$$
\boxed{\partial_t^2\left(w_{xx}+w_{zz}-\frac2H w_z+\frac1{H^2}w\right)+N^2w_{xx}=0,}
$$

which differs from the requested equation. The factor two arises when differentiating both $\rho_0$ and $w_z-w/H$. Keeping variable [density](../../../../density.md) in continuity while treating it as constant during that differentiation would be inconsistent.

For the intended [anelastic reduced-pressure Kelvin wave](../../../../anelastic-reduced-pressure-kelvin-wave.md), make the explicit correction $w_t-b+\Phi_z=0$, while $u_t+\Phi_x=0$ and $\Phi=p'/\rho_0$. Continuity then gives $\Phi_{xx}=w_{zt}-w_t/H$, and vertical momentum gives $w_{tt}+N^2w=-\Phi_{zt}$. Cross differentiation now produces

$$
\boxed{\partial_t^2\left(w_{xx}+w_{zz}-\frac1H w_z\right)+N^2w_{xx}=0.}
$$

This proves the advertised equation for the corrected model, without claiming it follows from the incompatible printed set.

A concrete counterexample makes the distinction testable. In nondimensional units $H=N=k=1$, take $m=0$, $\omega=2/\sqrt5$ and $w=e^{z/2}e^{i(x-\omega t)}$, multiplied by its [Gaussian meridional envelope](../../../../equatorial-kelvin-wave.md). This satisfies the last boxed wave equation, but substitution into the literal printed-system wave operator gives $-2w/5\ne0$. No choice of accompanying [pressure](../../../../pressure-split.md) and horizontal velocity can then make it a solution of all five printed equations. Conversely, the literal operator has vertical factors $e^{z/H+imz}$ and dispersion $\omega^2=N^2k^2/(k^2+m^2)$; its scaling is different from the requested half-scale-height factor.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
