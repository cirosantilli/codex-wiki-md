<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First eliminate the density-dependent definition of the auxiliary $\mathbf g$. The [Newtonian gravitational stress tensor](../../../../../../newtonian-gravitational-stress-tensor.md) can be written without derivatives of its normalization:

$$
T_{ij}=\frac1{4\pi G}\left(\partial_i\Phi\,\partial_j\Phi-\frac12\delta_{ij}\partial_k\Phi\,\partial_k\Phi\right).
$$

Here $\delta_{ij}$ is the [Kronecker delta](../../../../../../kronecker-delta.md), and repeated indices are summed. Differentiating gives

$$
\partial_jT_{ij}=\frac1{4\pi G}\left(\partial_j\partial_i\Phi\,\partial_j\Phi+\partial_i\Phi\,\nabla^2\Phi-\partial_k\Phi\,\partial_i\partial_k\Phi\right)
=\frac{\partial_i\Phi}{4\pi G}\nabla^2\Phi=\rho\partial_i\Phi.
$$

The first and third terms cancel because mixed [partial derivatives](../../../../../../partial-derivative.md) commute; the final step uses the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md). Therefore **the gravitational force density is a stress divergence**:

$$
\boxed{-\rho\nabla\Phi=-\nabla\cdot\mathbf T.}
$$

The identity holds for spatially varying [mass density](../../../../../../density.md): substituting the definition of $\mathbf g$ before differentiating prevents erroneous extra density-gradient terms.

For the [gravitational stress contribution to angular-momentum transport](../../../../../../gravitational-stress-contribution-to-angular-momentum-transport.md), the anisotropic term $\rho g_i g_j$ supplies [angular momentum transport](../../../../../../angular-momentum-transport.md). In cylindrical components its radial–azimuthal entry is

$$
T_{r\phi}=\frac{\partial_r\Phi\,(r^{-1}\partial_\phi\Phi)}{4\pi G}=\rho g_rg_\phi.
$$

In the momentum conservation equation, $rT_{r\phi}$ is the radial stress contribution to the [angular-momentum flux](../../../../../../angular-momentum-flux.md), whose sign depends on the correlated radial and azimuthal field components. It vanishes for a perfectly axisymmetric potential but can be nonzero for spiral disturbances.

The other term is isotropic and acts as an effective negative [pressure](../../../../../../pressure.md), $P_g=-\rho g^2/2=-|\nabla\Phi|^2/(8\pi G)$. Its force contribution is $-\nabla P_g=+\nabla(\rho g^2/2)$, modifying normal compression and force balance. It has no off-diagonal shear component and therefore no direct radial [angular momentum transport](../../../../../../angular-momentum-transport.md). In an axisymmetric averaged disk it supplies no azimuthal torque. The complete symmetric [Newtonian gravitational stress tensor](../../../../../../newtonian-gravitational-stress-tensor.md) also expresses [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) without an internal couple.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
