<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $B_0=B_z>0$, $v_a=B_0/\sqrt{\mu_0\rho_0}$ and $\zeta=k(z-v_at)$. The transverse [ideal magnetohydrodynamic induction equation](../../../../../../../ideal-magnetohydrodynamic-induction-equation.md) and [magnetohydrodynamic momentum equation](../../../../../../../magnetohydrodynamic-momentum-equation.md) are satisfied by $u_x=-B_x/\sqrt{\mu_0\rho_0}$, $u_y=u_z=0$, with constant [mass density](../../../../../../../density.md). However, the longitudinal [magnetohydrodynamic momentum equation](../../../../../../../magnetohydrodynamic-momentum-equation.md) also requires

$$
0=-\partial_z\left(p+\frac{B_x^2}{2\mu_0}\right).
$$

Here $B_x^2=a^2B_0^2\cos^2\zeta$ is not constant. Balancing its [gradient](../../../../../../../gradient.md) would require

$$
p=p_*(t)-\frac{a^2B_0^2}{2\mu_0}\cos^2\zeta.
$$

The adiabatic [pressure](../../../../../../../pressure.md) equation instead gives $\partial_t p=0$, since this [velocity](../../../../../../../velocity.md) is divergence-free and has no component along the spatial variation. No choice of $p_*(t)$ removes the spatially varying time derivative. Thus **a nontrivial finite-amplitude linearly polarized sinusoidal [Alfvén wave](../../../../../../../alfven-wave.md) is not an exact pure traveling wave in a compressible ideal fluid.** The [magnetic-pressure obstruction to a linearly polarized Alfvén wave](../../../../../../../magnetic-pressure-obstruction-to-a-linearly-polarized-alfven-wave.md) is quadratic in $a$, so the wave is a valid linear approximation and drives a compressive response at higher order. In an incompressible model [pressure](../../../../../../../pressure.md) is a constraint variable; it is not governed by the same compressible adiabatic evolution law.

Allowing longitudinal flow and varying [mass density](../../../../../../../density.md) does not rescue a regular one-dimensional periodic traveling solution with precisely this transverse [magnetic field](../../../../../../../magnetic-field.md). To see this, let $U=u_z-v_a$ and use the traveling coordinate. Integrated continuity, induction and transverse momentum give

$$
\rho U=m,\qquad UB_x-B_0u_x=A,\qquad
mu_x-\frac{B_0B_x}{\mu_0}=D,
$$

where $m,A,D$ are constants. Eliminating $u_x$ gives

$$
\left(\frac{m^2}{\rho}-\frac{B_0^2}{\mu_0}\right)B_x=mA+B_0D.
$$

At any zero of $B_x$, finite [mass density](../../../../../../../density.md) and [velocity](../../../../../../../velocity.md) require the right side to vanish. Wherever $B_x\ne0$, the coefficient then vanishes and fixes $\rho=\mu_0m^2/B_0^2$, constant; continuity fixes $U$, and adiabatic [entropy](../../../../../../../entropy.md) transport fixes $p$. The longitudinal [magnetohydrodynamic momentum equation](../../../../../../../magnetohydrodynamic-momentum-equation.md) again contradicts the varying $B_x^2$. The alternative $m=0$ makes transverse momentum force $B_x$ constant. Trivial cases such as $a=0$ or $k=0$ are excluded from the nontrivial wave conclusion.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
