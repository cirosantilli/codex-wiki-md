<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In the ideal, leading anisotropic system, there are **five separately conserved quadratic cascade quantities**: the two oppositely propagating Alfvén populations, the two slow-wave populations, and the [entropy](../../../../../../entropy.md) fluctuation. With the amplitudes of part (b), one convenient normalization is

$$
\boxed{I_A^\pm=\int|\mathbf z_\perp^\pm|^2dV,\qquad I_S^\pm=\int(f^\pm)^2dV,\qquad I_e=\int s^2dV,}
$$

where $\mathbf z_\perp^\pm=\mathbf u_\perp\pm\delta\mathbf B_\perp/\sqrt{4\pi\rho_0}$. Constant background factors convert the [velocity](../../../../../../velocity.md) [variances](../../../../../../variance-split.md) into modal energies and the [entropy](../../../../../../entropy.md) [variance](../../../../../../variance-split.md) into an entropy-related free-energy contribution. These are the [five quadratic cascade invariants of anisotropic magnetohydrodynamic turbulence](../../../../../../five-quadratic-cascade-invariants-of-anisotropic-magnetohydrodynamic-turbulence.md).

To verify conservation rather than just count polarizations, the perpendicular [Elsässer variables](../../../../../../elsasser-variable.md) obey

$$
\partial_t\mathbf z_\perp^\pm\mp v_A\partial_z\mathbf z_\perp^\pm+(\mathbf z_\perp^\mp\cdot\nabla_\perp)\mathbf z_\perp^\pm=-\nabla_\perp\Pi,\qquad\nabla_\perp\cdot\mathbf z_\perp^\pm=0.
$$

Dot each equation with $2\mathbf z_\perp^\pm$ and integrate. The propagation and nonlinear terms become surface fluxes of $|\mathbf z_\perp^\pm|^2$, and the [pressure](../../../../../../pressure.md) term becomes a surface flux because the corresponding field is [solenoidal](../../../../../../solenoidal-vector-field.md). For periodic boundaries, or boundaries with vanishing invariant flux, all these terms vanish and $dI_A^\pm/dt=0$. Their sum is proportional to perpendicular kinetic plus [magnetic energy](../../../../../../magnetic-energy.md), while their difference is proportional to perpendicular [cross-helicity](../../../../../../cross-helicity.md); the two [Elsässer energy invariants](../../../../../../elsasser-energy-invariant.md) contain both pieces of information.

Likewise the slow-mode equations give

$$
\frac{dI_S^\pm}{dt}=-\int\mathbf u_\perp\cdot\nabla_\perp(f^\pm)^2dV\mp c_T\int\nabla_\parallel(f^\pm)^2dV=0.
$$

Here $\mathbf u_\perp$ is [divergence-free](../../../../../../solenoidal-vector-field.md) and $\nabla_\parallel$ differentiates along the [divergence-free](../../../../../../solenoidal-vector-field.md) [vector](../../../../../../vector.md) $\hat{\mathbf z}+\delta\mathbf B_\perp/B_0$, so both integrals are boundary fluxes. Finally $Ds=0$ gives $dI_e/dt=-\int\mathbf u_\perp\cdot\nabla_\perp s^2dV=0$. This proves all five quadratic [conservation laws](../../../../../../conservation-law.md) under the same boundary assumptions.

The two Alfvén cascades interact dynamically: each population strains the other and is needed for its nonlinear transfer between scales. Their integrated invariants are nevertheless conserved separately, so this interaction does not transfer one population's invariant into the other. The slow and [entropy](../../../../../../entropy.md) cascades are driven by the Alfvénic mixing and field-line motion, with no feedback on the perpendicular cascade at the retained order. Their injection rates set independent fluxes; those fluxes need not be equal, even when the resulting perpendicular spectra share the $-5/3$ scaling.

The count is a count of independent quadratic modal cascade channels. Ideal passive advection also preserves higher moments, such as $\int F(s)dV$ for arbitrary smooth $F$, and analogous integrals for the slow characteristic scalars. These are not additional quadratic modal energies. Forcing and dissipative terms make the corresponding invariants source-and-sink balances; a stationary [inertial range](../../../../../../inertial-range.md) conserves their flux through scales rather than their total content in a continually forced domain.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
