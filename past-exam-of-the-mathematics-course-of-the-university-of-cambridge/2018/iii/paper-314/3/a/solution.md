<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $A=\Phi_0R_0^\beta<0$, $q=\lambda^2$ and $s=R^2+qz^2$. The [flattened power-law gravitational potential](../../../../../../flattened-power-law-gravitational-potential.md) is $\Phi=As^{-\beta/2}$. In axisymmetric [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md), the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) gives

$$
4\pi G\rho=\frac1R\partial_R(R\partial_R\Phi)+\partial_z^2\Phi.
$$

The first derivatives are $\partial_R\Phi=-\beta ARs^{-(\beta+2)/2}$ and $\partial_z\Phi=-\beta Aqzs^{-(\beta+2)/2}$. Differentiating again and collecting powers gives

$$
\nabla^2\Phi=-\beta As^{-(\beta+4)/2}\left[(2+q)s-(\beta+2)(R^2+q^2z^2)\right].
$$

Therefore the required [mass density](../../../../../../density.md) is

$$
\boxed{\rho(R,z)=-\frac{\beta\Phi_0R_0^\beta}{4\pi G}\frac{(\lambda^2-\beta)R^2+\lambda^2[2-(\beta+1)\lambda^2]z^2}{(R^2+\lambda^2z^2)^{(\beta+4)/2}}.}
$$

This is a formal density for arbitrary $\lambda$, but a physical [dark matter](../../../../../../dark-matter.md) distribution must be nonnegative. The [density positivity for a flattened power-law potential](../../../../../../density-positivity-for-a-flattened-power-law-potential.md) condition is

$$
\boxed{\beta\leq\lambda^2\leq\frac2{\beta+1}.}
$$

Necessity follows by evaluating on the midplane and symmetry axis; sufficiency follows because both numerator coefficients are then nonnegative. In this range the origin is a locally integrable density cusp: the mass enclosed near radius $r$ scales as $r^{1-\beta}$ and tends to zero, so no point mass needs adding. The scale-free distribution has infinite total mass at large radius and represents an idealized background, not a finite isolated halo.

For the cold, non-self-gravitating disk, radial balance of a [circular orbit](../../../../../../circular-orbit.md) is $R\Omega^2=\partial_R\Phi(R,0)$. Thus

$$
\boxed{\Omega^2(R)=-\beta\Phi_0R_0^\beta R^{-\beta-2},\qquad\Omega(R)=\frac{\sqrt{-\beta\Phi_0}}{R_0}\left(\frac R{R_0}\right)^{-(\beta+2)/2}.}
$$

The displayed positive root chooses the rotation orientation; the opposite orientation has the negative of this angular frequency.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
