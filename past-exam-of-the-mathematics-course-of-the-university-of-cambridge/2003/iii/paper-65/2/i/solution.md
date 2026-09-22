<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume an axisymmetric [thin disk](../../../../../../thin-disk.md) in the fixed [Newtonian potential of a point mass](../../../../../../newtonian-potential-of-a-point-mass.md), negligible disk self-gravity, and slow evolution compared with an orbital period. Radial pressure and radial inertia are small compared with gravity and centrifugal acceleration, so $u_\phi=r\Omega(r)$ with $\Omega=(GM/r^3)^{1/2}$, independent of height and time. Assume no mass loss or torque through the upper and lower disk faces. Define the [surface density of a disk](../../../../../../surface-density-of-a-disk.md), mass-weighted radial velocity and integrated shear stress by

$$
\Sigma=\int\rho\,dz,\qquad \Sigma\bar u_r=\int\rho u_r\,dz,\qquad W=\int T_{r\phi}\,dz.
$$

Vertical integration of the [continuity equation](../../../../../../continuity-equation.md) gives

$$
\partial_t\Sigma+\frac1r\partial_r(r\Sigma\bar u_r)=0.
$$

The azimuthal momentum equation, including the geometric term $u_ru_\phi/r$, gives [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) in terms of $j=r^2\Omega$:

$$
\partial_t(\Sigma j)+\frac1r\partial_r(r\Sigma\bar u_rj)=\frac1r\partial_r(r^2W).
$$

Subtracting $j$ times mass conservation eliminates the time derivative and leaves $\Sigma\bar u_rj'=r^{-1}(r^2W)'$.

Define the effective [density-weighted viscosity of a disk](../../../../../../density-weighted-viscosity-of-a-disk.md) through the actual stress:

$$
\boxed{W=\bar\nu\Sigma r\Omega',\qquad
\bar\nu=\frac{\int T_{r\phi}\,dz}{\Sigma r\Omega'}}.
$$

If the local viscous stress is $T_{r\phi}=\rho\nu r\Omega'$, this reduces to $\bar\nu=\Sigma^{-1}\int\rho\nu\,dz$. The definition can also describe an effective turbulent transport stress, provided the same shear closure is appropriate. Since $\Omega'<0$, outward transport corresponds to $W<0$ and positive $\bar\nu$.

For [Keplerian rotation](../../../../../../keplerian-disk.md), $j=\sqrt{GMr}$ and $r^2W=-(3/2)\sqrt{GM}\,r^{1/2}\bar\nu\Sigma$. Therefore

$$
\boxed{\bar u_r=-\frac3{\Sigma r^{1/2}}\partial_r(r^{1/2}\bar\nu\Sigma)}.
$$

Substitution into mass conservation yields the [Keplerian viscous diffusion equation](../../../../../../keplerian-viscous-diffusion-equation.md)

$$
\boxed{\partial_t\Sigma=\frac3r\partial_r\left[r^{1/2}\partial_r(r^{1/2}\bar\nu\Sigma)\right]}.
$$

The absence of surface fluxes, fixed rotation law and leading thin-disk approximation are essential: a wind, appreciable radial inertia or evolving gravitational potential would alter this reduction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
