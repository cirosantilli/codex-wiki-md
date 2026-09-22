<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $S(R)$ for the genuine [surface density of a disk](../../../../../surface-density-of-a-disk.md), and $\rho(R,z)=S(R)\delta(z)$ for its three-dimensional [mass density](../../../../../density.md). The delta function in the printed [surface density](../../../../../surface-density-of-a-disk.md) formula belongs to $\rho$, not to $S$. Introduce a reference length $R_*$ to make logarithms dimensionless. The intended model is the infinite, self-gravitating, scale-free [Mestel disk](../../../../../mestel-disk.md), with no extra source or imposed gravitational field.

The [circular speed](../../../../../circular-speed.md) satisfies $v_c^2=R\partial_R\Phi(R,0)$. Thus the flat [galaxy rotation curve](../../../../../galaxy-rotation-curve.md) gives

$$
\Phi(R,0)=v_0^2\log(R/R_*).
$$

A reflection-symmetric [harmonic function](../../../../../harmonic-function.md) with this midplane boundary value is

$$
\boxed{\Phi(R,z)=v_0^2\log\frac{\sqrt{R^2+z^2}+|z|}{R_*}.}
$$

Verify this continuation using the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md). For $z>0$, set $r=\sqrt{R^2+z^2}$; then

$$
\Phi_R=\frac{v_0^2}{R}\left(1-\frac zr\right),\qquad
\Phi_z=\frac{v_0^2}{r},\qquad
\frac1R\partial_R(R\Phi_R)=\frac{v_0^2z}{r^3},\qquad
\Phi_{zz}=-\frac{v_0^2z}{r^3}.
$$

Hence $\nabla^2\Phi=0$ off the [astrophysical disk](../../../../../astrophysical-disk.md), and reflection gives the lower-half-space solution. Across the [astrophysical disk](../../../../../astrophysical-disk.md) the derivative jumps by $\Phi_z(0^+)-\Phi_z(0^-)=2v_0^2/R$. The distributional [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) therefore gives

$$
\boxed{S(R)=\frac{v_0^2}{2\pi GR},\qquad
\rho(R,z)=\frac{v_0^2}{2\pi GR}\delta(z).}
$$

At the origin the enclosed disk [mass](../../../../../mass.md) tends to zero linearly with radius, so there is no additional central [point mass](../../../../../point-mass.md). This verifies the [Mestel disk potential-density pair](../../../../../mestel-disk-potential-density-pair.md). The [astrophysical disk](../../../../../astrophysical-disk.md) has infinite total [mass](../../../../../mass.md) and a logarithmic [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md), so it is not an isolated finite-mass model with [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) zero at infinity. The usual scale-free boundary condition is important: the midplane rotation curve alone would also permit an added term $a|z|$, representing an extra uniform sheet without changing the radial circular [force](../../../../../force.md). That contribution is excluded in the intended [Mestel disk](../../../../../mestel-disk.md) model.

Use a mass-weighted planar [galactic distribution function](../../../../../galactic-distribution-function.md), so $F(\boldsymbol x,\boldsymbol v)d^2x\,d^2v$ is the stellar [mass](../../../../../mass.md) in a small planar [phase space](../../../../../phase-space.md) element. A number-weighted function instead needs the stellar [mass](../../../../../mass.md) factor when computing $S$. Assume a steady [collisionless stellar system](../../../../../collisionless-stellar-system.md) and isotropy in the two in-plane [velocity](../../../../../velocity.md) components. Put $u=|\boldsymbol v|^2/2$ and write $F=f(\boldsymbol x,u)$. The stationary [Collisionless Boltzmann equation](../../../../../collisionless-boltzmann-equation.md) becomes

$$
\boldsymbol v\cdot\left(\nabla_x f-f_u\nabla_x\Phi\right)=0.
$$

Since this holds in every [velocity](../../../../../velocity.md) direction, $\nabla_x f=f_u\nabla_x\Phi$. In coordinates $(\boldsymbol x,E)$ with $E=u+\Phi$, this is exactly $\nabla_x f|_E=0$. Therefore **the [planar isotropic distribution](../../../../../planar-isotropic-stellar-distribution-function.md) is $F(E)$**, where $E$ is the [specific orbital energy](../../../../../specific-orbital-energy.md). Stationarity is essential; instantaneous isotropy alone would not imply this result.

Integrating over the two-dimensional [velocity](../../../../../velocity.md) plane gives the [planar isotropic distribution inversion](../../../../../planar-isotropic-distribution-inversion.md):

$$
S(R)=\int_{\mathbb R^2}F\!\left(\Phi+\frac{v^2}{2}\right)d^2v
=2\pi\int_0^\infty F(\Phi+v^2/2)\,v\,dv
=2\pi\int_\Phi^\infty F(E)\,dE.
$$

On the [astrophysical disk](../../../../../astrophysical-disk.md) $R=R_*e^{\Phi/v_0^2}$, so $S(\Phi)=v_0^2e^{-\Phi/v_0^2}/(2\pi GR_*)$. Differentiate the integral with respect to its lower limit:

$$
F(\Phi)=-\frac1{2\pi}\frac{dS}{d\Phi},\qquad
\boxed{F(E)=\frac1{4\pi^2GR_*}e^{-E/v_0^2}.}
$$

The boundary value $S\to0$ as $\Phi\to\infty$ verifies the integrated equation as well as its derivative. Choosing the implicit length unit $R_*=1$ recovers the printed normalization. Changing the additive [energy](../../../../../energy.md) zero changes this prefactor accordingly.

At a fixed radius, the normalized [velocity](../../../../../velocity.md) density is

$$
\frac{F(E)}{S(R)}=
\frac1{2\pi v_0^2}\exp\left[-\frac{v_R^2+v_\phi^2}{2v_0^2}\right].
$$

It is a product of centered [Gaussian distributions](../../../../../normal-distribution.md). Differentiating the supplied [Gaussian integral](../../../../../gaussian-integral.md) with respect to its coefficient gives the second moments, and odd moments vanish. Thus the in-plane [velocity dispersions](../../../../../velocity-dispersion.md) are

$$
\boxed{\sigma_R^2=\sigma_\phi^2=v_0^2,\qquad
\langle v_Rv_\phi\rangle=0,\qquad \langle v_\phi\rangle=0.}
$$

An exactly planar [astrophysical disk](../../../../../astrophysical-disk.md) has $v_z=0$ and $\sigma_z=0$. The nonzero [circular speed](../../../../../circular-speed.md) is a property of the [force](../../../../../force.md) field, not a statement that this hot stellar distribution has net rotation.

Reversing every retrograde [star](../../../../../star.md) folds the azimuthal Gaussian to a [half-normal distribution](../../../../../half-normal-distribution.md). Equivalently the new steady [galactic distribution function](../../../../../galactic-distribution-function.md) is $F_+(E,L_z)=2F(E)\Theta(L_z)$, because $E$ and $L_z=Rv_\phi$ are integrals of the motion. Its density and even [velocity](../../../../../velocity.md) moments are unchanged. Its [streaming velocity](../../../../../streaming-velocity.md) is

$$
\boxed{\langle v_\phi\rangle_+=\langle|v_\phi|\rangle
=\frac{2}{\sqrt{2\pi}v_0}\int_0^\infty v_\phi e^{-v_\phi^2/(2v_0^2)}dv_\phi
=\sqrt{\frac2\pi}\,v_0.}
$$

This [maximally prograde stellar distribution](../../../../../maximally-prograde-stellar-distribution.md) still has radial motion and a spread of azimuthal [speeds](../../../../../speed.md); it does not place every [star](../../../../../star.md) on a [circular orbit](../../../../../circular-orbit.md). In particular $\langle v_\phi^2\rangle_+=v_0^2$ while $\sigma_{\phi,+}^2=v_0^2(1-2/\pi)$. The mean [speed](../../../../../speed.md) is smaller than the root-mean-square [speed](../../../../../speed.md) $v_0$, which explains why it is not the [circular speed](../../../../../circular-speed.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
