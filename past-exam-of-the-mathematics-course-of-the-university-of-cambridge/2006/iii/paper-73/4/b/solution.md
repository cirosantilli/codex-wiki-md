<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First consider a genuinely one-dimensional, time-independent [collisionless stellar system](../../../../../../collisionless-stellar-system.md) with [Hamiltonian](../../../../../../hamiltonian.md) $E_z=v_z^2/2+\psi(z)$. Choose $\psi(0)=0$. For bound vertical oscillations, a phase-mixed population has equal occupations of the upward and downward branches of each orbit. By [Jeans theorem](../../../../../../jeans-theorem.md), its stationary distribution is a function of the conserved vertical energy, $f_z(z,v_z)=F_z(E_z)$. Equivalently, the one-dimensional [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) $v_z\partial_z f_z-\psi'(z)\partial_{v_z}f_z=0$ makes $f_z$ constant along the energy curves. Branch-dependent incoming and outgoing populations or time-dependent waves would not satisfy this assumption.

Integrate both signs of $v_z$ and change variable to $E=v_z^2/2+\psi$:

$$
\nu(\psi)=2\int_0^\infty F_z\!\left(\psi+\frac{v_z^2}{2}\right)dv_z=\sqrt2\int_\psi^\infty\frac{F_z(E)}{\sqrt{E-\psi}}\,dE.
$$

The density is thus an [Abel transform](../../../../../../abel-transform.md) of the vertical-energy distribution. To invert it without simply quoting an inversion rule, apply a second integral and exchange its order:

$$
J(E)=\int_E^\infty\frac{\nu(\psi)}{\sqrt{\psi-E}}\,d\psi=\sqrt2\int_E^\infty F_z(t)\,dt\int_E^t\frac{d\psi}{\sqrt{(t-\psi)(\psi-E)}}=\pi\sqrt2\int_E^\infty F_z(t)\,dt.
$$

The inner integral is $\pi$, as follows by setting $\psi=E+(t-E)\sin^2\theta$. Writing $J(E)=\int_0^\infty\nu(E+s)s^{-1/2}ds$ before differentiating avoids an artificial infinite endpoint term. Under sufficient differentiability and decay,

$$
J'(E)=\int_E^\infty\frac{d\nu/d\psi}{\sqrt{\psi-E}}\,d\psi=-\pi\sqrt2F_z(E).
$$

The [vertical-energy Abel inversion of a stellar distribution](../../../../../../vertical-energy-abel-inversion-of-a-stellar-distribution.md) is therefore

$$
\boxed{F_z(E_z)=\frac1\pi\int_{E_z}^\infty\frac{-d\nu/d\psi}{\sqrt{2(\psi-E_z)}}\,d\psi.}
$$

This proves the normalization, including the factor from the two velocity signs. The additive origin of $\psi$ merely changes the origin of energy.

For this expression to define a physical [phase-space distribution function](../../../../../../phase-space-distribution-function.md), $\nu$ must be expressible as a single-valued function of $\psi$, the integrals and differentiated integral must converge, and the resulting $F_z$ must be nonnegative. Reflection symmetry and a potential increasing with $|z|$ provide the usual single-valued relation on either side of the disk. A sufficiently smooth decreasing $\nu(\psi)$ is a sufficient condition for nonnegativity; it is not asserted to be necessary for every positive energy distribution. If there is a finite escape energy, replace the infinite limits by that energy and impose the appropriate cutoff and boundary conditions. The displayed infinite-limit formula presumes either a confining potential or a distribution extended by zero above its allowed energy, with no omitted boundary population.

A three-dimensional [galactic disk](../../../../../../galactic-disk.md) does not automatically meet these hypotheses. Exact separation $\Phi(R,z)=\Phi_{\parallel}(R)+\psi(z)$ makes $E_z$ an [integral of motion](../../../../../../integral-of-motion.md). If the full [galactic distribution function](../../../../../../galactic-distribution-function.md) factorizes into an in-plane factor and a vertical factor $F_z(E_z)$, integrating the in-plane velocities gives the required one-dimensional distribution after its normalization is absorbed into $\nu$. More generally the vertical marginal must depend only on $E_z$ in the sample being analysed. Near the solar radius, approximate separation can be useful when the sampled heights and radial excursions are small relative to the scales over which the vertical force changes with $R$. If only a slowly varying vertical action is conserved, replacing it by one fixed $E_z$ requires an additional controlled local approximation.

The population must be sufficiently stationary and phase mixed, with negligible mean vertical flow, and the data must measure a well-defined tracer population with a known selection function. Radial coupling and the tilted [velocity ellipsoid](../../../../../../velocity-ellipsoid.md) must be negligible or modelled. In the full [vertical Jeans equation](../../../../../../vertical-jeans-equation.md), that coupling is $R^{-1}\partial_R(R\nu\overline{v_Rv_z})$; it cannot generally be discarded merely because a mixed moment vanishes at the midplane. The tracer [number density](../../../../../../number-density.md) $\nu$ is not the [mass density](../../../../../../density.md) producing the potential.

To infer the local mass, measure the tracer density as a function of height and its vertical velocity distribution near the midplane. With $\psi(0)=0$, the latter directly samples $F_z(v_z^2/2)$. Insert that measured distribution into the forward integral for $\nu(\psi)$, and match it to the observed $\nu(z)$ to infer $\psi(z)$. Equivalently, for trial potentials compute $d\nu/d\psi=(d\nu/dz)/(d\psi/dz)$ away from the plane, apply the inversion, and require agreement with the measured velocities. Density data alone do not determine both an unknown potential and an unknown energy distribution.

Once the vertical force is known, use the full axisymmetric [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md), rather than identifying every vertical derivative with density in isolation:

$$
4\pi G\rho_{\rm tot}(R,z)=\partial_z^2\Phi+\frac1R\partial_R(R\partial_R\Phi).
$$

At the midplane, $v_c^2(R)=R\partial_R\Phi(R,0)$, so

$$
\boxed{\rho_{\rm tot}(R_0,0)=\frac1{4\pi G}\left[\psi''(0)+\frac1{R_0}\frac{dv_c^2}{dR}\bigg|_{R_0}\right].}
$$

In terms of the circular-orbit [Oort constants](../../../../../../oort-constants.md), $A=\tfrac12(v_c/R-dv_c/dR)$ and $B=-\tfrac12(v_c/R+dv_c/dR)$, the radial term equals $2(B^2-A^2)$. It vanishes for a locally flat [rotation curve](../../../../../../galaxy-rotation-curve.md), not for an arbitrary rotating disk. An integrated version gives the [dynamical surface density from vertical stellar motions](../../../../../../dynamical-surface-density-from-vertical-stellar-motions.md):

$$
2\pi G\Sigma_{\rm tot}(<|z|)=\psi'(z)+\int_0^z\frac1{R_0}\partial_R(R\partial_R\Phi)\big|_{R_0,z'}\,dz'\qquad(z>0).
$$

Here the actual vertical acceleration is $-\psi'(z)$. The sign of the radial correction follows directly from the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md).

For an illustrative isothermal tracer with constant vertical [velocity dispersion](../../../../../../velocity-dispersion.md) $s$, take

$$
F_z(E)=\frac{\nu_0}{\sqrt{2\pi}\,s}e^{-E/s^2}.
$$

The velocity integral gives $\nu(z)=\nu_0e^{-\psi(z)/s^2}$, hence $\psi(z)=-s^2\ln[\nu(z)/\nu_0]$. For a locally flat [rotation curve](../../../../../../galaxy-rotation-curve.md) this yields

$$
\rho_{\rm tot}(R_0,0)=-\frac{s^2}{4\pi G}\frac{d^2\ln\nu}{dz^2}\bigg|_0.
$$

This example shows explicitly how a measured tracer scale and velocity scale constrain the gravitating density; using the tracer's own density as the mass source would instead impose an unjustified self-gravitating model.

The inferred density includes luminous and faint [stars](../../../../../../star.md), gas and [dark matter](../../../../../../dark-matter.md). Comparing it with an independently estimated baryonic census tests for extra gravitating mass. An excess need not be a dark disk: a [dark matter halo](../../../../../../dark-matter-halo.md) also contributes to the local force. Conversely, agreement with the baryonic density locally does not exclude a halo at other radii or heights. Vertical disequilibrium, radial mixing, errors in selection or tracer populations, and neglected velocity tilt can mimic a mass discrepancy, so the one-dimensional equilibrium assumptions must be tested when interpreting such an inference.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
