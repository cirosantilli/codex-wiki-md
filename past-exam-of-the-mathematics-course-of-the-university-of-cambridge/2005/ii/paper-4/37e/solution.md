<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

For an incompressible [Newtonian fluid](../../../../../newtonian-fluid.md) the [viscous stress](../../../../../viscous-stress-tensor.md) is $\tau_{ij}=2\mu e_{ij}$, where $e_{ij}=(u_{i,j}+u_{j,i})/2$. Its work converted to heat per unit volume is $\tau_{ij}u_{i,j}$. The antisymmetric part of the velocity gradient has zero contraction with symmetric $e_{ij}$, so

$$
\boxed{\Phi=2\mu e_{ij}e_{ij}\ge0}.
$$

For [potential flow](../../../../../potential-flow.md), $u_i=\phi_{,i}$ and mixed [derivatives](../../../../../derivative.md) commute, giving $e_{ij}=\phi_{,ij}$ and $\Phi=2\mu\sum_{i,j}\phi_{,ij}^2$.

Use the given linear wave potential with $z$ increasing downward and $\theta=kx-\omega t$. The nonzero strain components are

$$
e_{xx}=\omega ak e^{-kz}\sin\theta,\qquad
e_{zz}=-\omega ak e^{-kz}\sin\theta,\qquad
e_{xz}=e_{zx}=\omega ak e^{-kz}\cos\theta.
$$

Their squared contraction is $2\omega^2a^2k^2e^{-2kz}$, independent of the phase. Thus the time-averaged dissipation density is

$$
\boxed{\overline\Phi=4\mu\omega^2a^2k^2e^{-2kz}}.
$$

Depth integration gives dissipation $2\mu\omega^2a^2k$ per unit horizontal area, or $4\pi\mu\omega^2a^2$ per wavelength and unit transverse width.

The velocity components are $u_x=-\omega ae^{-kz}\cos\theta$ and $u_z=\omega ae^{-kz}\sin\theta$. Hence the depth-integrated mean [kinetic energy](../../../../../kinetic-energy.md) per wavelength is

$$
\boxed{\overline K=\frac{\rho}{2}\frac{2\pi}{k}
\int_0^\infty\omega^2a^2e^{-2kz}\,dz
=\frac{\pi\rho\omega^2a^2}{2k^2}}.
$$

Equal mean potential and [kinetic energies](../../../../../kinetic-energy.md) give total [energy](../../../../../energy.md) $\mathcal E=\pi\rho\omega^2a^2/k^2$. Dividing the dissipation by that [energy](../../../../../energy.md) yields

$$
\boxed{\dot{\mathcal E}=-\frac{4\mu k^2}{\rho}\mathcal E,\qquad
\mathcal E(t)\sim\mathcal E(0)e^{-4\mu k^2t/\rho}}.
$$

The amplitude decays at half this exponent. The small-viscosity and deep-water assumptions justify evaluating the leading dissipation in the inviscid wave field, extending the depth to infinity and neglecting higher-order amplitude corrections.

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
