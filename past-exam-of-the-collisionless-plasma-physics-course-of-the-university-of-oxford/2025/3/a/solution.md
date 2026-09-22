<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [Gaussian units](../../../../gaussian-units.md) and the [kinetic magnetohydrodynamics](../../../../kinetic-magnetohydrodynamics.md) equations

$$
\partial_t\mathbf B=\nabla\times(\mathbf u\times\mathbf B),\qquad
\rho D_t\mathbf u=-\nabla\cdot\mathbf P+\frac{(\nabla\times\mathbf B)\times\mathbf B}{4\pi},\qquad
\mathbf P=p_\perp\mathbf I+(p_\parallel-p_\perp)\mathbf b\mathbf b,
$$

together with species [continuity equations](../../../../continuity-equation.md), [quasineutrality](../../../../quasineutrality.md) and the [drift-kinetic equation](../../../../drift-kinetic-equation.md). Here $p_\perp,p_\parallel$ sum the species [pressures](../../../../pressure-split.md). Interpret the [thermal speed](../../../../thermal-speed.md) denominator in the source as the species [mass](../../../../mass.md) $m_\alpha$, so $v_{\mathrm{th}\alpha}^2=2T_{0\alpha}/m_\alpha$ and the [first adiabatic invariant](../../../../first-adiabatic-invariant.md) is $\mu=v_\perp^2/(2B)$.

The specified [Maxwell-Boltzmann distribution](../../../../maxwell-boltzmann-distribution.md) has zero mean motion and [isotropic](../../../../isotropy.md) [pressure](../../../../pressure-split.md), $p_{\perp0}=p_{\parallel0}=p_0$. All equilibrium scalars depend only on $x$, while $\mathbf b_0\cdot\nabla x=0$ and $\mathbf b_0\cdot\nabla B_0=0$. Therefore the equilibrium streaming and mirror terms of the [drift-kinetic equation](../../../../drift-kinetic-equation.md) vanish. The remaining terms vanish because $\mathbf u_0=0$ and $E_{\parallel0}=0$; the parallel electric constraint is also satisfied because the equilibrium parallel [pressure gradient](../../../../pressure-gradient.md) is zero. Species [continuity equations](../../../../continuity-equation.md) and the induction equation are stationary, and [quasineutrality](../../../../quasineutrality.md) holds by assumption.

It remains to check the perpendicular [force balance](../../../../force-balance.md). The radial [magnetic pressure](../../../../magnetic-pressure.md) and [magnetic tension](../../../../magnetic-tension.md) give

$$
0=-\frac{dp_0}{dx}-\frac{d}{dx}\frac{B_0^2}{8\pi}-\frac{B_0^2}{4\pi R}
=\frac{p_0}{L_p}+\frac{B_0^2}{4\pi L_B}-\frac{B_0^2}{4\pi R}.
$$

This is precisely

$$
\boxed{\frac1R-\frac1{L_B}=\frac{4\pi p_0}{B_0^2L_p}=\frac\beta{2L_p}.}
$$

Thus the [Z-pinch](../../../../z-pinch.md) is a steady solution of the stated [kinetic magnetohydrodynamics](../../../../kinetic-magnetohydrodynamics.md) system. Its equilibrium [electric current](../../../../electric-current.md) is supplied by the small species drifts implicit in this approximation; zero leading common flow does not require zero [electric current](../../../../electric-current.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
