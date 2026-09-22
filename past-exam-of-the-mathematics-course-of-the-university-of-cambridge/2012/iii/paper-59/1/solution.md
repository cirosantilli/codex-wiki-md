<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $V=|v_0|>0$, take $q>0$ without loss of generality, and write $s=R^2+z^2/q^2$. The [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) is singular at the origin; all pointwise claims below concern $s>0$. The zero of the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) is the one in the paper, with an implicit fixed length unit inside the [logarithm](../../../../../logarithm.md).

The [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) in [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md) gives

$$
4\pi G\rho=\frac1R\partial_R(R\Phi_R)+\Phi_{zz},\qquad \Phi_R=\frac{V^2R}{s},\qquad \Phi_z=\frac{V^2z}{q^2s}.
$$

The two contributions to the [Laplacian](../../../../../laplacian.md) are

$$
\frac1R\partial_R(R\Phi_R)=\frac{2V^2}{s}-\frac{2V^2R^2}{s^2},\qquad \Phi_{zz}=\frac{V^2}{q^2s}-\frac{2V^2z^2}{q^4s^2}.
$$

Consequently the [mass density](../../../../../density.md) of the [axisymmetric logarithmic gravitational potential](../../../../../axisymmetric-logarithmic-gravitational-potential.md) is

$$
\boxed{\rho(R,z)=\frac{V^2}{4\pi Gq^2}\frac{R^2+(2-q^{-2})z^2}{(R^2+q^{-2}z^2)^2}.}
$$

The coefficient of $R^2$ is positive. The coefficient of $z^2$ determines the [density positivity for an axisymmetric logarithmic potential](../../../../../density-positivity-for-an-axisymmetric-logarithmic-potential.md): **strict positivity at every noncentral point requires $q^2>1/2$ and $v_0\ne0$**. Nonnegativity permits $q^2=1/2$, where the [mass density](../../../../../density.md) vanishes on the noncentral symmetry axis. For $q^2<1/2$ it is negative near that axis. Either sign of a nonzero real $q$ gives the same model, and $q=0$ is undefined. Setting $v_0=0$ yields vacuum away from the singular origin, not strictly positive [mass density](../../../../../density.md). The $r^{-2}$ central cusp is locally integrable and contains no hidden point [mass](../../../../../mass.md): the [Newtonian gravitational field](../../../../../newtonian-gravitational-field.md) flux through a shrinking sphere is of order its radius.

An equatorial [circular orbit](../../../../../circular-orbit.md) requires inward [gravitational acceleration](../../../../../gravitational-acceleration.md) equal to $v_c^2/R$. Thus the [circular speed](../../../../../circular-speed.md) is

$$
v_c^2=R\Phi_R(R,0)=V^2,\qquad \boxed{v_c(R)=V\quad(R>0).}
$$

This is a [flat galaxy rotation curve](../../../../../flat-galaxy-rotation-curve.md). The singular center does not define an additional circular orbit at $R=0$.

<a id="1/image-flat-equatorial-rotation-curve-of-the-singular-logarithmic-galaxy-the-central-point-is-excluded"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-59-rotation-curve.png)

**[Figure 1](#1/image-flat-equatorial-rotation-curve-of-the-singular-logarithmic-galaxy-the-central-point-is-excluded). Flat equatorial rotation curve of the singular logarithmic galaxy; the central point is excluded**.

The [specific orbital energy](../../../../../specific-orbital-energy.md) $E=\tfrac12(v_R^2+v_\phi^2+v_z^2)+\Phi$ is conserved because the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) is time independent. The axial [specific angular momentum](../../../../../specific-angular-momentum.md) $L_z=Rv_\phi$ is conserved because the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) is axisymmetric. Hence the [Jeans theorem](../../../../../jeans-theorem.md), or directly $dF(E,L_z^2)/dt=0$ in the [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md), permits a stationary [two-integral galactic distribution function](../../../../../two-integral-galactic-distribution-function.md). Using $L_z^2$ makes this [galactic distribution function](../../../../../galactic-distribution-function.md) even under reversal of the azimuthal [velocity](../../../../../velocity.md), so it describes a nonstreaming population. A general axisymmetric population can have an odd part in $L_z$, or dependence on a third [integral of motion](../../../../../integral-of-motion.md); neither is required for this construction.

At each position define $\rho\langle g\rangle=\int gF\,d^3v$. The [two-integral galactic distribution function](../../../../../two-integral-galactic-distribution-function.md) is invariant under swapping $v_R$ and $v_z$, since only their sum of squares occurs in $E$. It is also even in each [velocity](../../../../../velocity.md) component. Swapping integration variables proves [meridional velocity isotropy of a two-integral distribution](../../../../../meridional-velocity-isotropy-of-a-two-integral-distribution.md), while reflecting one variable makes each mixed integrand odd. Therefore

$$
\boxed{\langle v_R^2\rangle=\langle v_z^2\rangle,\qquad \langle v_Rv_z\rangle=\langle v_Rv_\phi\rangle=\langle v_\phi v_z\rangle=0.}
$$

All mean [velocities](../../../../../velocity.md) vanish, so these are also the corresponding statements for the [velocity ellipsoid](../../../../../velocity-ellipsoid.md) and its centered [covariance](../../../../../covariance.md) tensor. They do not require $\langle v_\phi^2\rangle$ to equal either meridional second moment.

To normalize the proposed [logarithmic-potential two-integral distribution](../../../../../logarithmic-potential-two-integral-distribution.md), first separate the [mass density](../../../../../density.md) into terms with the same spatial factors as the two exponentials:

$$
\rho=\frac{V^2}{4\pi Gq^2}\left[\frac{2q^2-1}{s}+\frac{2(1-q^2)R^2}{s^2}\right].
$$

Since $e^{-2\Phi/V^2}=s^{-1}$ and $e^{-4\Phi/V^2}=s^{-2}$, the [Gaussian integral](../../../../../gaussian-integral.md) and its derivative give

$$
\int e^{-v^2/V^2}\,d^3v=\pi^{3/2}V^3,\qquad \int v_\phi^2e^{-2v^2/V^2}\,d^3v=\frac{\pi^{3/2}V^5}{8\sqrt2}.
$$

Thus velocity integration of the [galactic distribution function](../../../../../galactic-distribution-function.md) yields $AR^2s^{-2}\pi^{3/2}V^5/(8\sqrt2)+Bs^{-1}\pi^{3/2}V^3$. Matching the independent spatial factors determines

$$
\boxed{A=\frac{4\sqrt2(1-q^2)}{\pi^{5/2}Gq^2V^3},\qquad B=\frac{2q^2-1}{4\pi^{5/2}Gq^2V}.}
$$

This verifies both the stationary [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) and the required [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md). A shift $\Phi\mapsto\Phi+C$ changes the normalizations to $Ae^{4C/V^2}$ and $Be^{2C/V^2}$; the physical [mass density](../../../../../density.md) is unchanged.

There is an important distinction between positive [mass density](../../../../../density.md) and a nonnegative [galactic distribution function](../../../../../galactic-distribution-function.md). For $1/2\le q^2\le1$, both coefficients above are nonnegative. For a prolate model $q^2>1$, $A<0$ and one must test the sum rather than reject the model just because one term is negative. On accessible phase space,

$$
L_z^2e^{-2E/V^2}=\frac{R^2}{s}v_\phi^2e^{-v^2/V^2}\le\frac{V^2}{e},
$$

with equality in the equatorial plane at $v_R=v_z=0$, $v_\phi^2=V^2$. The [nonnegativity bound for a prolate logarithmic-potential distribution](../../../../../nonnegativity-bound-for-a-prolate-logarithmic-potential-distribution.md) is consequently

$$
\boxed{q^2\le\frac{16\sqrt2-e}{16\sqrt2-2e}\quad(q^2>1).}
$$

For larger $q$, the displayed algebraic expression still integrates to the positive [mass density](../../../../../density.md), but is negative at those equatorial [circular orbit](../../../../../circular-orbit.md) phase points and is not a physical [galactic distribution function](../../../../../galactic-distribution-function.md). This extra restriction is distinct from the earlier density-only answer.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
