<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In an axisymmetric [cylindrical coordinate system](../../../../../../cylindrical-coordinate-system.md), the steady [Collisionless Boltzmann equation](../../../../../../collisionless-boltzmann-equation.md) is

$$
v_R\frac{\partial f}{\partial R}+v_z\frac{\partial f}{\partial z}+\left(\frac{v_\phi^2}{R}-\Phi_R\right)\frac{\partial f}{\partial v_R}-\frac{v_Rv_\phi}{R}\frac{\partial f}{\partial v_\phi}-\Phi_z\frac{\partial f}{\partial v_z}=0.
$$

Let $\nu=\int f\,d^3v$ and $\overline A=\nu^{-1}\int Af\,d^3v$. Multiply by $v_R$ and integrate over velocities. The spatial terms give $\partial_R(\nu\overline{v_R^2})+\partial_z(\nu\overline{v_Rv_z})$. [Integration by parts](../../../../../../integration-by-parts.md) in $v_R$ supplies $\nu\Phi_R-\nu\overline{v_\phi^2}/R$, and the $v_\phi$ derivative supplies $\nu\overline{v_R^2}/R$. The $v_z$ force term vanishes because $v_R$ does not depend on $v_z$. This assumes sufficient decay of the [galactic distribution function](../../../../../../galactic-distribution-function.md) to discard all velocity boundary terms. The radial [Jeans equation](../../../../../../jeans-equation.md) is consequently

$$
\partial_R(\nu\overline{v_R^2})+\partial_z(\nu\overline{v_Rv_z})+\frac{\nu}{R}(\overline{v_R^2}-\overline{v_\phi^2})+\nu\Phi_R=0.
$$

Reflection symmetry about $z=0$ makes $\nu$ even and $\overline{v_Rv_z}$ odd. At the midplane the latter vanishes, and $\nu^{-1}\partial_z(\nu\overline{v_Rv_z})=\partial_z\overline{v_Rv_z}$. Multiplying by $R/\nu$ proves

$$
\boxed{\frac R\nu\partial_R(\nu\overline{v_R^2})+R\partial_z\overline{v_Rv_z}+\overline{v_R^2}-\overline{v_\phi^2}+R\Phi_R=0\quad(z=0).}
$$

All quadratic velocities here are population moments, not individual stellar velocities. In particular, symmetry does not make the [midplane tilt contribution to asymmetric drift](../../../../../../midplane-tilt-contribution-to-asymmetric-drift.md) disappear: an odd mixed moment can have a nonzero derivative at zero.

For application to the [Milky Way](../../../../../../milky-way.md), assume negligible mean radial and vertical flows, and define the circular [speed](../../../../../../speed.md) by $v_c^2=R\Phi_R(R,0)$. Write $\overline{v_R^2}=\sigma_R^2$ and $\overline{v_\phi^2}=\overline v_\phi^{\,2}+\sigma_\phi^2$. Rearranging gives the exact stress-support relation

$$
\boxed{v_c^2-\overline v_\phi^{\,2}=\sigma_R^2\left[-\frac{d\ln(\nu\sigma_R^2)}{d\ln R}-1+\frac{\sigma_\phi^2}{\sigma_R^2}\right]-R\partial_z\overline{v_Rv_z}\big|_0.}
$$

Thus the [stellar asymmetric drift](../../../../../../stellar-asymmetric-drift.md) $v_a=v_c-\overline v_\phi$ is the right-hand side divided by $v_c+\overline v_\phi$. For $v_a\ll v_c$, this denominator is approximately $2v_c$. If $\nu\propto e^{-R/h_\nu}$ and $\sigma_R^2\propto e^{-R/h_\sigma}$ locally, the bracket becomes $R/h_\nu+R/h_\sigma-1+\sigma_\phi^2/\sigma_R^2$, making the density and dispersion-gradient contributions explicit.

A radially declining random-motion stress supplies some of the force needed to support a [galactic disk](../../../../../../galactic-disk.md), so its stars need less ordered azimuthal motion than a population on circular orbits. Hotter, often older, [stellar populations](../../../../../../stellar-population.md) therefore generally rotate more slowly than cold populations in the same [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md); this is the observed [stellar asymmetric drift](../../../../../../stellar-asymmetric-drift.md). It is a stress-support effect, not a frictional slowing of each orbit. For a [velocity ellipsoid](../../../../../../velocity-ellipsoid.md) aligned approximately with spherical coordinates, $\overline{v_Rv_z}\simeq(\sigma_R^2-\sigma_z^2)z/R$, and the midplane tilt term contributes $-(\sigma_R^2-\sigma_z^2)$ rather than zero.

Local measurements of mean rotation and all components of the [velocity dispersion](../../../../../../velocity-dispersion.md), combined with tracer-density and dispersion gradients, can therefore constrain $v_c$ and the radial [Newtonian gravitational field](../../../../../../newtonian-gravitational-field.md). A hotter sample's mean rotation must not be identified directly with the circular [speed](../../../../../../speed.md). The tracer [number density](../../../../../../number-density.md) need not be the gravitating [mass density](../../../../../../density.md). Nonaxisymmetric streaming, a nonstationary disk, poorly measured radial gradients, or a neglected tilt term can bias this inference; these are assumptions of the derivation rather than extra free corrections to the circular force.

## ↑ Ancestors (11)

1. [A](../a.md)
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
